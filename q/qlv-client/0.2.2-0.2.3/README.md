# Comparing `tmp/qlv-client-0.2.2.tar.gz` & `tmp/qlv-client-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qlv-client-0.2.2.tar", last modified: Fri May 10 03:48:14 2024, max compression
+gzip compressed data, was "qlv-client-0.2.3.tar", last modified: Fri May 10 03:54:29 2024, max compression
```

## Comparing `qlv-client-0.2.2.tar` & `qlv-client-0.2.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-05-10 03:48:14.380742 qlv-client-0.2.2/
--rw-rw-rw-   0        0        0    11558 2024-04-17 06:55:59.000000 qlv-client-0.2.2/LICENSE
--rw-rw-rw-   0        0        0      456 2024-05-10 03:48:14.380245 qlv-client-0.2.2/PKG-INFO
--rw-rw-rw-   0        0        0       11 2024-04-17 06:55:59.000000 qlv-client-0.2.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-10 03:48:14.377762 qlv-client-0.2.2/qlv_client/
--rw-rw-rw-   0        0        0      463 2024-04-17 08:02:13.000000 qlv-client-0.2.2/qlv_client/__init__.py
--rw-rw-rw-   0        0        0     9543 2024-04-17 08:27:22.000000 qlv-client-0.2.2/qlv_client/api.py
--rw-rw-rw-   0        0        0     1224 2024-04-17 07:59:59.000000 qlv-client-0.2.2/qlv_client/config.py
--rw-rw-rw-   0        0        0     1303 2024-04-17 07:30:16.000000 qlv-client-0.2.2/qlv_client/converter.py
--rw-rw-rw-   0        0        0     4115 2024-04-29 09:06:57.000000 qlv-client-0.2.2/qlv_client/http_client.py
--rw-rw-rw-   0        0        0    10097 2024-05-10 03:48:03.000000 qlv-client-0.2.2/qlv_client/proxy.py
--rw-rw-rw-   0        0        0     3187 2024-04-17 08:27:22.000000 qlv-client-0.2.2/qlv_client/repository.py
--rw-rw-rw-   0        0        0     2235 2024-04-17 08:27:22.000000 qlv-client-0.2.2/qlv_client/test.py
--rw-rw-rw-   0        0        0     1995 2024-04-17 07:29:50.000000 qlv-client-0.2.2/qlv_client/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-10 03:48:14.379748 qlv-client-0.2.2/qlv_client.egg-info/
--rw-rw-rw-   0        0        0      456 2024-05-10 03:48:14.000000 qlv-client-0.2.2/qlv_client.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      391 2024-05-10 03:48:14.000000 qlv-client-0.2.2/qlv_client.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-10 03:48:14.000000 qlv-client-0.2.2/qlv_client.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-05-10 03:48:14.000000 qlv-client-0.2.2/qlv_client.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-10 03:48:14.000000 qlv-client-0.2.2/qlv_client.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-10 03:48:14.380742 qlv-client-0.2.2/setup.cfg
--rw-rw-rw-   0        0        0     1066 2024-05-10 03:48:10.000000 qlv-client-0.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-10 03:54:29.925753 qlv-client-0.2.3/
+-rw-rw-rw-   0        0        0    11558 2024-04-17 06:55:59.000000 qlv-client-0.2.3/LICENSE
+-rw-rw-rw-   0        0        0      456 2024-05-10 03:54:29.925257 qlv-client-0.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0       11 2024-04-17 06:55:59.000000 qlv-client-0.2.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-10 03:54:29.922773 qlv-client-0.2.3/qlv_client/
+-rw-rw-rw-   0        0        0      463 2024-04-17 08:02:13.000000 qlv-client-0.2.3/qlv_client/__init__.py
+-rw-rw-rw-   0        0        0     9543 2024-04-17 08:27:22.000000 qlv-client-0.2.3/qlv_client/api.py
+-rw-rw-rw-   0        0        0     1224 2024-04-17 07:59:59.000000 qlv-client-0.2.3/qlv_client/config.py
+-rw-rw-rw-   0        0        0     1303 2024-04-17 07:30:16.000000 qlv-client-0.2.3/qlv_client/converter.py
+-rw-rw-rw-   0        0        0     4115 2024-04-29 09:06:57.000000 qlv-client-0.2.3/qlv_client/http_client.py
+-rw-rw-rw-   0        0        0    10291 2024-05-10 03:54:21.000000 qlv-client-0.2.3/qlv_client/proxy.py
+-rw-rw-rw-   0        0        0     3187 2024-04-17 08:27:22.000000 qlv-client-0.2.3/qlv_client/repository.py
+-rw-rw-rw-   0        0        0     2235 2024-04-17 08:27:22.000000 qlv-client-0.2.3/qlv_client/test.py
+-rw-rw-rw-   0        0        0     1995 2024-04-17 07:29:50.000000 qlv-client-0.2.3/qlv_client/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-10 03:54:29.924761 qlv-client-0.2.3/qlv_client.egg-info/
+-rw-rw-rw-   0        0        0      456 2024-05-10 03:54:29.000000 qlv-client-0.2.3/qlv_client.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      391 2024-05-10 03:54:29.000000 qlv-client-0.2.3/qlv_client.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-10 03:54:29.000000 qlv-client-0.2.3/qlv_client.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-05-10 03:54:29.000000 qlv-client-0.2.3/qlv_client.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-10 03:54:29.000000 qlv-client-0.2.3/qlv_client.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-10 03:54:29.925753 qlv-client-0.2.3/setup.cfg
+-rw-rw-rw-   0        0        0     1066 2024-05-10 03:54:25.000000 qlv-client-0.2.3/setup.py
```

### Comparing `qlv-client-0.2.2/LICENSE` & `qlv-client-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `qlv-client-0.2.2/qlv_client/api.py` & `qlv-client-0.2.3/qlv_client/api.py`

 * *Files identical despite different names*

### Comparing `qlv-client-0.2.2/qlv_client/config.py` & `qlv-client-0.2.3/qlv_client/config.py`

 * *Files identical despite different names*

### Comparing `qlv-client-0.2.2/qlv_client/converter.py` & `qlv-client-0.2.3/qlv_client/converter.py`

 * *Files identical despite different names*

### Comparing `qlv-client-0.2.2/qlv_client/http_client.py` & `qlv-client-0.2.3/qlv_client/http_client.py`

 * *Files identical despite different names*

### Comparing `qlv-client-0.2.2/qlv_client/proxy.py` & `qlv-client-0.2.3/qlv_client/proxy.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,16 +39,21 @@
         kwargs.update(unlock_order_params)
         order_ser = OrderService(**QlvConfigRepository.get_host_params())
         result = order_ser.unlock_order(**kwargs)
         if result.get("code") == 1:
             logger.info("劲旅平台订单<{}>解锁成功.".format(order_id))
             return True
         else:
-            logger.error(result)
-            return False
+            message = result.get("message")
+            if "解锁失败" in message:
+                # 说明订单是未锁定状态
+                return True
+            else:
+                logger.error(result)
+                return False
 
     @classmethod
     def unlock_reason_with_flag(cls, flag: bool, order_id: int, oper: str, remark: str) -> bool:
         unlock_reason_params = QlvConfigRepository.get_unlock_reason_params(
             flag=flag, order_id=order_id, oper=oper, remark=remark
         )
         return cls.set_unlock_order(**unlock_reason_params)
```

### Comparing `qlv-client-0.2.2/qlv_client/repository.py` & `qlv-client-0.2.3/qlv_client/repository.py`

 * *Files identical despite different names*

### Comparing `qlv-client-0.2.2/qlv_client/test.py` & `qlv-client-0.2.3/qlv_client/test.py`

 * *Files identical despite different names*

### Comparing `qlv-client-0.2.2/qlv_client/utils.py` & `qlv-client-0.2.3/qlv_client/utils.py`

 * *Files identical despite different names*

