# Comparing `tmp/qlv-client-0.1.9.tar.gz` & `tmp/qlv-client-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qlv-client-0.1.9.tar", last modified: Tue Apr 30 03:17:48 2024, max compression
+gzip compressed data, was "qlv-client-0.2.0.tar", last modified: Fri May 10 02:51:35 2024, max compression
```

## Comparing `qlv-client-0.1.9.tar` & `qlv-client-0.2.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-04-30 03:17:48.621360 qlv-client-0.1.9/
--rw-rw-rw-   0        0        0    11558 2024-04-17 06:55:59.000000 qlv-client-0.1.9/LICENSE
--rw-rw-rw-   0        0        0      456 2024-04-30 03:17:48.620863 qlv-client-0.1.9/PKG-INFO
--rw-rw-rw-   0        0        0       11 2024-04-17 06:55:59.000000 qlv-client-0.1.9/README.md
-drwxrwxrwx   0        0        0        0 2024-04-30 03:17:48.618379 qlv-client-0.1.9/qlv_client/
--rw-rw-rw-   0        0        0      463 2024-04-17 08:02:13.000000 qlv-client-0.1.9/qlv_client/__init__.py
--rw-rw-rw-   0        0        0     9543 2024-04-17 08:27:22.000000 qlv-client-0.1.9/qlv_client/api.py
--rw-rw-rw-   0        0        0     1224 2024-04-17 07:59:59.000000 qlv-client-0.1.9/qlv_client/config.py
--rw-rw-rw-   0        0        0     1303 2024-04-17 07:30:16.000000 qlv-client-0.1.9/qlv_client/converter.py
--rw-rw-rw-   0        0        0     4115 2024-04-29 09:06:57.000000 qlv-client-0.1.9/qlv_client/http_client.py
--rw-rw-rw-   0        0        0     6561 2024-04-30 03:17:22.000000 qlv-client-0.1.9/qlv_client/proxy.py
--rw-rw-rw-   0        0        0     3187 2024-04-17 08:27:22.000000 qlv-client-0.1.9/qlv_client/repository.py
--rw-rw-rw-   0        0        0     2235 2024-04-17 08:27:22.000000 qlv-client-0.1.9/qlv_client/test.py
--rw-rw-rw-   0        0        0     1995 2024-04-17 07:29:50.000000 qlv-client-0.1.9/qlv_client/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-30 03:17:48.620366 qlv-client-0.1.9/qlv_client.egg-info/
--rw-rw-rw-   0        0        0      456 2024-04-30 03:17:48.000000 qlv-client-0.1.9/qlv_client.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      391 2024-04-30 03:17:48.000000 qlv-client-0.1.9/qlv_client.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-30 03:17:48.000000 qlv-client-0.1.9/qlv_client.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-04-30 03:17:48.000000 qlv-client-0.1.9/qlv_client.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-04-30 03:17:48.000000 qlv-client-0.1.9/qlv_client.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-30 03:17:48.621360 qlv-client-0.1.9/setup.cfg
--rw-rw-rw-   0        0        0     1066 2024-04-30 03:15:52.000000 qlv-client-0.1.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-10 02:51:35.967662 qlv-client-0.2.0/
+-rw-rw-rw-   0        0        0    11558 2024-04-17 06:55:59.000000 qlv-client-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0      456 2024-05-10 02:51:35.967166 qlv-client-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0       11 2024-04-17 06:55:59.000000 qlv-client-0.2.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-10 02:51:35.964186 qlv-client-0.2.0/qlv_client/
+-rw-rw-rw-   0        0        0      463 2024-04-17 08:02:13.000000 qlv-client-0.2.0/qlv_client/__init__.py
+-rw-rw-rw-   0        0        0     9543 2024-04-17 08:27:22.000000 qlv-client-0.2.0/qlv_client/api.py
+-rw-rw-rw-   0        0        0     1224 2024-04-17 07:59:59.000000 qlv-client-0.2.0/qlv_client/config.py
+-rw-rw-rw-   0        0        0     1303 2024-04-17 07:30:16.000000 qlv-client-0.2.0/qlv_client/converter.py
+-rw-rw-rw-   0        0        0     4115 2024-04-29 09:06:57.000000 qlv-client-0.2.0/qlv_client/http_client.py
+-rw-rw-rw-   0        0        0     9342 2024-05-10 02:49:21.000000 qlv-client-0.2.0/qlv_client/proxy.py
+-rw-rw-rw-   0        0        0     3187 2024-04-17 08:27:22.000000 qlv-client-0.2.0/qlv_client/repository.py
+-rw-rw-rw-   0        0        0     2235 2024-04-17 08:27:22.000000 qlv-client-0.2.0/qlv_client/test.py
+-rw-rw-rw-   0        0        0     1995 2024-04-17 07:29:50.000000 qlv-client-0.2.0/qlv_client/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-10 02:51:35.966669 qlv-client-0.2.0/qlv_client.egg-info/
+-rw-rw-rw-   0        0        0      456 2024-05-10 02:51:35.000000 qlv-client-0.2.0/qlv_client.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      391 2024-05-10 02:51:35.000000 qlv-client-0.2.0/qlv_client.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-10 02:51:35.000000 qlv-client-0.2.0/qlv_client.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-05-10 02:51:35.000000 qlv-client-0.2.0/qlv_client.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-10 02:51:35.000000 qlv-client-0.2.0/qlv_client.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-10 02:51:35.967662 qlv-client-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1066 2024-05-10 02:29:11.000000 qlv-client-0.2.0/setup.py
```

### Comparing `qlv-client-0.1.9/LICENSE` & `qlv-client-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `qlv-client-0.1.9/qlv_client/api.py` & `qlv-client-0.2.0/qlv_client/api.py`

 * *Files identical despite different names*

### Comparing `qlv-client-0.1.9/qlv_client/config.py` & `qlv-client-0.2.0/qlv_client/config.py`

 * *Files identical despite different names*

### Comparing `qlv-client-0.1.9/qlv_client/converter.py` & `qlv-client-0.2.0/qlv_client/converter.py`

 * *Files identical despite different names*

### Comparing `qlv-client-0.1.9/qlv_client/http_client.py` & `qlv-client-0.2.0/qlv_client/http_client.py`

 * *Files identical despite different names*

### Comparing `qlv-client-0.1.9/qlv_client/proxy.py` & `qlv-client-0.2.0/qlv_client/proxy.py`

 * *Files 18% similar despite different names*

```diff
@@ -58,14 +58,33 @@
         # 尝试3次解锁
         for i in range(attempts):
             is_succeed = QlvService.unlock_reason_with_flag(flag=flag, order_id=order_id, oper=oper, remark=remark)
             if is_succeed is True:
                 break
 
     @classmethod
+    def set_system_unlock_order(cls, order_id: int, flag: bool, oper: str, remark: str) -> bool:
+        if flag is True:
+            order_state = "1"
+        else:
+            order_state = "0"
+        return cls.set_unlock_order(
+            order_id=order_id, oper=oper, order_state=order_state, order_lose_type="系统", remark=remark
+        )
+
+    @classmethod
+    def loop_set_unlock_order(cls, pre_order_id: int, flag: bool, oper: str, remark: str, attempts: int = 3) -> bool:
+        is_success = False
+        for _ in range(attempts):
+            is_success = cls.set_system_unlock_order(order_id=pre_order_id, flag=flag, oper=oper, remark=remark)
+            if is_success is True:
+                break
+        return is_success
+
+    @classmethod
     def save_pay_info(cls, **kwargs) -> bool:
         logger.info("开始向劲旅系统回填采购信息...")
         args = QlvConfigRepository.get_request_base_params(inter_name="save_order_pay_info")
         order_pay_info = QlvConfigRepository.get_order_pay_info(**kwargs)
         args.update(order_pay_info)
         order_ser = OrderService(**QlvConfigRepository.get_host_params())
         result = order_ser.save_order_pay_info(**args)
@@ -73,14 +92,43 @@
             logger.error(result)
             return False
         else:
             logger.error("向劲旅系统回填采购信息成功.")
             return True
 
     @classmethod
+    def save_payment_info(cls, **kwargs) -> bool:
+        logger.info("开始向劲旅系统回填采购信息...")
+        args = QlvConfigRepository.get_request_base_params(inter_name="save_order_pay_info")
+        order_pay_info = QlvConfigRepository.get_order_pay_info(**kwargs)
+        args.update(order_pay_info)
+        order_ser = OrderService(**QlvConfigRepository.get_host_params())
+        result = order_ser.save_order_pay_info(**args)
+        if result.get("code") == 0:
+            message = result.get("message") or ''
+            if message.find("支付保存") != -1:
+                # 说名已经出票完成，再回填采购信息，就成了改签
+                return True
+            else:
+                logger.error(result)
+                return False
+        else:
+            logger.error("向劲旅系统回填采购信息成功.")
+            return True
+
+    @classmethod
+    def loop_save_payment_info(cls, payment_info: dict, attempts: int = 3) -> bool:
+        flag = False
+        for _ in range(attempts):
+            flag = cls.save_payment_info(**payment_info)
+            if flag is True:
+                break
+        return flag
+
+    @classmethod
     def save_itinerary_info(cls, **kwargs) -> bool:
         logger.info("开始向劲旅系统回填乘客票单信息...")
         args = QlvConfigRepository.get_request_base_params(inter_name="fill_order_itinerary_info")
         order_itinerary_info = QlvConfigRepository.get_order_itinerary_info(**kwargs)
         args.update(order_itinerary_info)
         order_ser = OrderService(**QlvConfigRepository.get_host_params())
         result = order_ser.fill_order_itinerary_info(**args)
@@ -120,19 +168,40 @@
             else:
                 logger.info("向劲旅系统回填乘客票单信息成功.")
                 return True
         else:
             return False
 
     @classmethod
+    def loop_save_itinerary_info(cls, pre_order_id: int, itinerary_info: list, oper: str, attempts: int = 3) -> bool:
+        flag = False
+        for _ in range(attempts):
+            flag = cls.save_itinerary_info_by_batch_itinerary(
+                pre_order_id=pre_order_id, oper=oper, itinerary_info=itinerary_info
+
+            )
+            if flag is True:
+                break
+        return flag
+
+    @classmethod
     def save_new_log(cls, pre_order_id: int, oper: str, logs: str) -> bool:
         logger.info("开始向劲旅系统给订单<{}>记录新日志...".format(pre_order_id))
         args = QlvConfigRepository.get_request_base_params(inter_name="write_order_log_new")
         args.update(dict(order_id=pre_order_id, oper=oper, logs=logs))
         order_ser = OrderService(**QlvConfigRepository.get_host_params())
         result = order_ser.write_order_log_new(**args)
         if result.get("code") == 0:
             logger.error("向劲旅系统给订单<{}>记录新日志失败...".format(pre_order_id))
             return False
         else:
             logger.info("向劲旅系统给订单<{}>记录新日志成功.".format(pre_order_id))
             return True
+
+    @classmethod
+    def loop_save_order_new_log(cls, pre_order_id: int, logs: str, oper: str, attempts: int = 3) -> bool:
+        flag = False
+        for _ in range(attempts):
+            flag = cls.save_new_log(pre_order_id=pre_order_id, logs=logs, oper=oper)
+            if flag is True:
+                break
+        return flag
```

### Comparing `qlv-client-0.1.9/qlv_client/repository.py` & `qlv-client-0.2.0/qlv_client/repository.py`

 * *Files identical despite different names*

### Comparing `qlv-client-0.1.9/qlv_client/test.py` & `qlv-client-0.2.0/qlv_client/test.py`

 * *Files identical despite different names*

### Comparing `qlv-client-0.1.9/qlv_client/utils.py` & `qlv-client-0.2.0/qlv_client/utils.py`

 * *Files identical despite different names*

### Comparing `qlv-client-0.1.9/setup.py` & `qlv-client-0.2.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Copyright ©2011-2024. Hunan xxxxxxx Company limited. All rights reserved.
 # ---------------------------------------------------------------------------------------------------------
 """
 from setuptools import setup, find_packages
 
 setup(
     name='qlv-client',
-    version='0.1.9',
+    version='0.2.0',
     description='This is my qlv proxy qlv_client package',
     long_description='This is my qlv proxy qlv_client package',
     author='ckf10000',
     author_email='ckf10000@sina.com',
     url='https://github.com/ckf10000/qlvClient',
     packages=find_packages(),
     install_requires=[
```

