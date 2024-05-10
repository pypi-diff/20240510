# Comparing `tmp/anotify-0.0.8.tar.gz` & `tmp/anotify-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anotify-0.0.8.tar", last modified: Fri May 10 07:20:07 2024, max compression
+gzip compressed data, was "anotify-0.0.9.tar", last modified: Fri May 10 12:37:00 2024, max compression
```

## Comparing `anotify-0.0.8.tar` & `anotify-0.0.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 07:20:07.079323 anotify-0.0.8/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 07:20:07.079323 anotify-0.0.8/ANotify/
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-05-10 07:20:01.000000 anotify-0.0.8/ANotify/Nanpush.py
--rw-r--r--   0 runner    (1001) docker     (127)     2643 2024-05-10 07:20:01.000000 anotify-0.0.8/ANotify/Nemail.py
--rw-r--r--   0 runner    (1001) docker     (127)     5241 2024-05-10 07:20:01.000000 anotify-0.0.8/ANotify/Nfeishu.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-10 07:20:01.000000 anotify-0.0.8/ANotify/Niyuu.py
--rw-r--r--   0 runner    (1001) docker     (127)     1567 2024-05-10 07:20:01.000000 anotify-0.0.8/ANotify/Npushplus.py
--rw-r--r--   0 runner    (1001) docker     (127)      720 2024-05-10 07:20:01.000000 anotify-0.0.8/ANotify/Nserverchan.py
--rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-05-10 07:20:01.000000 anotify-0.0.8/ANotify/Ntelegram.py
--rw-r--r--   0 runner    (1001) docker     (127)     6128 2024-05-10 07:20:01.000000 anotify-0.0.8/ANotify/Nwecom.py
--rw-r--r--   0 runner    (1001) docker     (127)      850 2024-05-10 07:20:01.000000 anotify-0.0.8/ANotify/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-10 07:20:01.000000 anotify-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4690 2024-05-10 07:20:07.079323 anotify-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4254 2024-05-10 07:20:01.000000 anotify-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 07:20:07.079323 anotify-0.0.8/anotify.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4690 2024-05-10 07:20:07.000000 anotify-0.0.8/anotify.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      356 2024-05-10 07:20:07.000000 anotify-0.0.8/anotify.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 07:20:07.000000 anotify-0.0.8/anotify.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-10 07:20:07.000000 anotify-0.0.8/anotify.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-10 07:20:07.000000 anotify-0.0.8/anotify.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 07:20:07.079323 anotify-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-05-10 07:20:01.000000 anotify-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:37:00.735468 anotify-0.0.9/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:37:00.731468 anotify-0.0.9/ANotify/
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-05-10 12:36:56.000000 anotify-0.0.9/ANotify/Nanpush.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2643 2024-05-10 12:36:56.000000 anotify-0.0.9/ANotify/Nemail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5214 2024-05-10 12:36:56.000000 anotify-0.0.9/ANotify/Nfeishu.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-10 12:36:56.000000 anotify-0.0.9/ANotify/Niyuu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1567 2024-05-10 12:36:56.000000 anotify-0.0.9/ANotify/Npushplus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-05-10 12:36:56.000000 anotify-0.0.9/ANotify/Nserverchan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-05-10 12:36:56.000000 anotify-0.0.9/ANotify/Ntelegram.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8624 2024-05-10 12:36:56.000000 anotify-0.0.9/ANotify/Nwecom.py
+-rw-r--r--   0 runner    (1001) docker     (127)      850 2024-05-10 12:36:56.000000 anotify-0.0.9/ANotify/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-10 12:36:56.000000 anotify-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5045 2024-05-10 12:37:00.735468 anotify-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4609 2024-05-10 12:36:56.000000 anotify-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:37:00.735468 anotify-0.0.9/anotify.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5045 2024-05-10 12:37:00.000000 anotify-0.0.9/anotify.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-05-10 12:37:00.000000 anotify-0.0.9/anotify.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 12:37:00.000000 anotify-0.0.9/anotify.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-10 12:37:00.000000 anotify-0.0.9/anotify.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-10 12:37:00.000000 anotify-0.0.9/anotify.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 12:37:00.735468 anotify-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-05-10 12:36:56.000000 anotify-0.0.9/setup.py
```

### Comparing `anotify-0.0.8/ANotify/Nanpush.py` & `anotify-0.0.9/ANotify/Nanpush.py`

 * *Files identical despite different names*

### Comparing `anotify-0.0.8/ANotify/Nemail.py` & `anotify-0.0.9/ANotify/Nemail.py`

 * *Files identical despite different names*

### Comparing `anotify-0.0.8/ANotify/Nfeishu.py` & `anotify-0.0.9/ANotify/Nfeishu.py`

 * *Files 2% similar despite different names*

```diff
@@ -158,15 +158,15 @@
     APPSECRET = ''
     OPEN_ID = ''
     UNION_ID = ''
     USER_ID = ''
     CHAT_ID = ''
 
     feishu = FeishuNotify(appid=APPID, appsecret=APPSECRET)
-    # print(feishu.send_file(ReceiverType.OPEN_ID, OPEN_ID, "E:/Desktop/gpt/Cursor_Demo/test.png"))
+    # print(feishu.send_file(ReceiverType.OPEN_ID, OPEN_ID, "test.png"))
     # print(feishu.send_msg(ReceiverType.OPEN_ID, OPEN_ID, "Hello World!"))
     # print(feishu.send_msg(ReceiverType.UINION_ID, UNION_ID, "Hello World!"))
     # print(feishu.send_msg(ReceiverType.USER_ID, USER_ID, "Hello World!"))
     # print(feishu.send_msg(ReceiverType.CHAT_ID, CHAT_ID, "Hello World!"))
 
     # feishu_webhook = FeishuWebhookNotify(webhook_url="https://open.feishu.cn/open-apis/bot/v2/hook/xxxxxxxxxxx")
     # feishu_webhook.send_msg("Hello World!")
```

### Comparing `anotify-0.0.8/ANotify/Npushplus.py` & `anotify-0.0.9/ANotify/Npushplus.py`

 * *Files identical despite different names*

### Comparing `anotify-0.0.8/ANotify/Nserverchan.py` & `anotify-0.0.9/ANotify/Nserverchan.py`

 * *Files identical despite different names*

### Comparing `anotify-0.0.8/ANotify/Ntelegram.py` & `anotify-0.0.9/ANotify/Ntelegram.py`

 * *Files identical despite different names*

### Comparing `anotify-0.0.8/ANotify/Nwecom.py` & `anotify-0.0.9/ANotify/Nwecom.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import requests
 from enum import Enum
 import json
+import base64
+import hashlib
 
 
 class MediaType(Enum):
     image = 'image'
     voice = 'voice'
     video = 'video'
     file = 'file'
@@ -162,18 +164,96 @@
             "enable_duplicate_check": 0,
             "duplicate_check_interval": 1800
         }
         resp = requests.post(url, data=json.dumps(payload))
         resp.raise_for_status()
         return resp.json()
 
+class WxWebhookNotify:
+    def __init__(self, webhook_url):
+        self.webhook_url = webhook_url
+
+    def send_msg(self, msg):
+        url = self.webhook_url
+        playload = {
+            "msgtype": "text",
+            "text": {
+                "content": msg,
+                # "mentioned_list":["@all"],
+                # "mentioned_mobile_list":["@all"]
+            }
+        }
+
+        res = requests.post(url, data=json.dumps(playload))
+        return res.json()
+
+    def send_msg_markdown(self, msg):
+        url = self.webhook_url
+        playload = {
+            "msgtype": "markdown",
+            "markdown": {
+                "content": msg,
+                # "mentioned_list":["@all"],
+                # "mentioned_mobile_list":["@all"]
+            }
+        }
+
+        res = requests.post(url, data=json.dumps(playload))
+        return res.json()
+
+    def send_img(self, img_path):
+        url = self.webhook_url
+        img_base64, img_md5 = self.get_img_info(img_path)
+        playload = {
+            "msgtype": "image",
+            "image": {
+                "base64": img_base64,
+                "md5": img_md5
+            }
+        }
+
+        res = requests.post(url, data=json.dumps(playload))
+        return res.json()
+    def send_file(self, file_path):
+        url = self.webhook_url
+        playload = {
+            "msgtype": "file",
+            "file": {
+                "media_id": self.upload_media(file_path)
+            }
+        }
+
+        res = requests.post(url, data=json.dumps(playload))
+        return res.json()
+
+    def upload_media(self, file_path):
+        key = self.webhook_url.split("key=")[1]
+        url = f"https://qyapi.weixin.qq.com/cgi-bin/webhook/upload_media?key={key}&type=file"
+
+        files = {'file': open(file_path, 'rb')}
+        result = requests.post(url, files=files)
+        response = json.loads(result.text)
+        return response['media_id']
+
+    def get_img_info(self, img_path):
+        with open(img_path, 'rb') as f:
+            img = f.read()
+            md5 = hashlib.md5(img).hexdigest()
+            img_base64 = base64.b64encode(img).decode('utf-8')
+        return img_base64, md5
 
 if __name__ == "__main__":
     # 企业ID
     CORPID = ''
     # 应用Secret
     CORPSECRET = ''
     # 应用ID
     AgentId = ''
 
-    wn = WxNotify(corpid=CORPID, corpsecret=CORPSECRET, agentid=AgentId)
-    print(wn.send_msg("test message"))
+    # wn = WxNotify(corpid=CORPID, corpsecret=CORPSECRET, agentid=AgentId)
+    # print(wn.send_msg("test message"))
+
+    wn_webhook = WxWebhookNotify("")
+    # wn_webhook.send_file("E:/Desktop/gpt/Cursor_Demo/test.png")
+    # wn_webhook.send_msg("Hello")
+    # print(wn_webhook.send_msg_markdown("**Hello**\n- test1\n- [ANotify](https://www.baidu.com)"))
+    # wn_webhook.send_img("E:/Desktop/gpt/Cursor_Demo/test.png")
```

### Comparing `anotify-0.0.8/ANotify/__init__.py` & `anotify-0.0.9/ANotify/__init__.py`

 * *Files identical despite different names*

### Comparing `anotify-0.0.8/LICENSE` & `anotify-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `anotify-0.0.8/PKG-INFO` & `anotify-0.0.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anotify
-Version: 0.0.8
+Version: 0.0.9
 Summary: Send notifications by multiple channels.
 Home-page: https://github.com/TommyMerlin/ANotify
 Author: 7ommy
 Author-email: tommymerlin0920@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -33,14 +33,22 @@
 AgentId = ''
 
 wn = Nwecom.WxNotify(corpid=CORPID, corpsecret=CORPSECRET, agentid=AgentId)
 wn.send_msg("test message")
 wn.send_text_card("test title", "test content", "https://www.example.com")
 wn.send_file("./test.txt")
 wn.send_img("./test.png")
+
+# Webhook
+WEB_HOOK = "https://qyapi.weixin.qq.com/cgi-bin/webhook/send?key=xxxxxx"
+wn_webhook = Nwecom.WxWebhookNotify(WEB_HOOK)
+wn_webhook.send_msg("Hello")
+wn_webhook.send_msg_markdown("**Hello**\n- test1\n- [ANotify](https://github.com/TommyMerlin/ANotify)")
+wn_webhook.send_img("E:/Desktop/gpt/Cursor_Demo/test.png")
+wn_webhook.send_file("test.png")
 ```
 
 ### 飞书
 [官网](https://open.feishu.cn/document/server-docs/im-v1/introduction)  
 [创建应用](https://open.feishu.cn/document/home/introduction-to-custom-app-development/self-built-application-development-process)  
 [API调试台](https://open.feishu.cn/api-explorer?from=op_doc_tab)  
 [获取消息发送对象 openid](https://open.feishu.cn/document/faq/trouble-shooting/how-to-obtain-openid)
```

#### html2text {}

```diff
@@ -1,21 +1,26 @@
-Metadata-Version: 2.1 Name: anotify Version: 0.0.8 Summary: Send notifications
+Metadata-Version: 2.1 Name: anotify Version: 0.0.9 Summary: Send notifications
 by multiple channels. Home-page: https://github.com/TommyMerlin/ANotify Author:
 7ommy Author-email: tommymerlin0920@gmail.com License: MIT Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Requires-Python: >=3.6 Description-Content-Type: text/markdown License-
 File: LICENSE Requires-Dist: requests>=2.15.1 ![Alt](https://
 repobeats.axiom.co/api/embed/e1ca45165d69b8370c78d60260a6474b49621fac.svg
 "Repobeats analytics image") ## å®è£ ```console pip install anotify ``` ##
 å®ä¾ ### ä¼ä¸å¾®ä¿¡ [å®ç½](https://work.weixin.qq.com/) ```python from
 ANotify import Nwecom # ä¼ä¸ID CORPID = '' # åºç¨Secret CORPSECRET = '' #
 åºç¨ID AgentId = '' wn = Nwecom.WxNotify(corpid=CORPID,
 corpsecret=CORPSECRET, agentid=AgentId) wn.send_msg("test message")
 wn.send_text_card("test title", "test content", "https://www.example.com")
-wn.send_file("./test.txt") wn.send_img("./test.png") ``` ### é£ä¹¦ [å®ç½]
+wn.send_file("./test.txt") wn.send_img("./test.png") # Webhook WEB_HOOK =
+"https://qyapi.weixin.qq.com/cgi-bin/webhook/send?key=xxxxxx" wn_webhook =
+Nwecom.WxWebhookNotify(WEB_HOOK) wn_webhook.send_msg("Hello")
+wn_webhook.send_msg_markdown("**Hello**\n- test1\n- [ANotify](https://
+github.com/TommyMerlin/ANotify)") wn_webhook.send_img("E:/Desktop/gpt/
+Cursor_Demo/test.png") wn_webhook.send_file("test.png") ``` ### é£ä¹¦ [å®ç½]
 (https://open.feishu.cn/document/server-docs/im-v1/introduction) [åå»ºåºç¨]
 (https://open.feishu.cn/document/home/introduction-to-custom-app-development/
 self-built-application-development-process) [APIè°è¯å°](https://
 open.feishu.cn/api-explorer?from=op_doc_tab) [è·åæ¶æ¯åéå¯¹è±¡ openid]
 (https://open.feishu.cn/document/faq/trouble-shooting/how-to-obtain-openid)
 [Webhookè¯·æ±åéæ¶æ¯](https://open.feishu.cn/document/client-docs/bot-v3/
 add-custom-bot#355ec8c0) ```python from ANotify import Nfeishu APPID = ''
```

### Comparing `anotify-0.0.8/README.md` & `anotify-0.0.9/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -18,14 +18,22 @@
 AgentId = ''
 
 wn = Nwecom.WxNotify(corpid=CORPID, corpsecret=CORPSECRET, agentid=AgentId)
 wn.send_msg("test message")
 wn.send_text_card("test title", "test content", "https://www.example.com")
 wn.send_file("./test.txt")
 wn.send_img("./test.png")
+
+# Webhook
+WEB_HOOK = "https://qyapi.weixin.qq.com/cgi-bin/webhook/send?key=xxxxxx"
+wn_webhook = Nwecom.WxWebhookNotify(WEB_HOOK)
+wn_webhook.send_msg("Hello")
+wn_webhook.send_msg_markdown("**Hello**\n- test1\n- [ANotify](https://github.com/TommyMerlin/ANotify)")
+wn_webhook.send_img("E:/Desktop/gpt/Cursor_Demo/test.png")
+wn_webhook.send_file("test.png")
 ```
 
 ### 飞书
 [官网](https://open.feishu.cn/document/server-docs/im-v1/introduction)  
 [创建应用](https://open.feishu.cn/document/home/introduction-to-custom-app-development/self-built-application-development-process)  
 [API调试台](https://open.feishu.cn/api-explorer?from=op_doc_tab)  
 [获取消息发送对象 openid](https://open.feishu.cn/document/faq/trouble-shooting/how-to-obtain-openid)
```

#### html2text {}

```diff
@@ -2,18 +2,23 @@
 e1ca45165d69b8370c78d60260a6474b49621fac.svg "Repobeats analytics image") ##
 å®è£ ```console pip install anotify ``` ## å®ä¾ ### ä¼ä¸å¾®ä¿¡ [å®ç½]
 (https://work.weixin.qq.com/) ```python from ANotify import Nwecom # ä¼ä¸ID
 CORPID = '' # åºç¨Secret CORPSECRET = '' # åºç¨ID AgentId = '' wn =
 Nwecom.WxNotify(corpid=CORPID, corpsecret=CORPSECRET, agentid=AgentId)
 wn.send_msg("test message") wn.send_text_card("test title", "test content",
 "https://www.example.com") wn.send_file("./test.txt") wn.send_img("./test.png")
-``` ### é£ä¹¦ [å®ç½](https://open.feishu.cn/document/server-docs/im-v1/
-introduction) [åå»ºåºç¨](https://open.feishu.cn/document/home/introduction-
-to-custom-app-development/self-built-application-development-process)
-[APIè°è¯å°](https://open.feishu.cn/api-explorer?from=op_doc_tab)
+# Webhook WEB_HOOK = "https://qyapi.weixin.qq.com/cgi-bin/webhook/
+send?key=xxxxxx" wn_webhook = Nwecom.WxWebhookNotify(WEB_HOOK)
+wn_webhook.send_msg("Hello") wn_webhook.send_msg_markdown("**Hello**\n-
+test1\n- [ANotify](https://github.com/TommyMerlin/ANotify)")
+wn_webhook.send_img("E:/Desktop/gpt/Cursor_Demo/test.png") wn_webhook.send_file
+("test.png") ``` ### é£ä¹¦ [å®ç½](https://open.feishu.cn/document/server-
+docs/im-v1/introduction) [åå»ºåºç¨](https://open.feishu.cn/document/home/
+introduction-to-custom-app-development/self-built-application-development-
+process) [APIè°è¯å°](https://open.feishu.cn/api-explorer?from=op_doc_tab)
 [è·åæ¶æ¯åéå¯¹è±¡ openid](https://open.feishu.cn/document/faq/trouble-
 shooting/how-to-obtain-openid) [Webhookè¯·æ±åéæ¶æ¯](https://
 open.feishu.cn/document/client-docs/bot-v3/add-custom-bot#355ec8c0) ```python
 from ANotify import Nfeishu APPID = '' APPSECRET = '' OPEN_ID = '' UNION_ID =
 '' USER_ID = '' CHAT_ID = '' feishu = Nfeishu.FeishuNotify(appid=APPID,
 appsecret=APPSECRET) feishu.send_msg(Nfeishu.ReceiverType.OPEN_ID, OPEN_ID,
 "Hello World!") feishu.send_msg(Nfeishu.ReceiverType.UINION_ID, UNION_ID,
```

### Comparing `anotify-0.0.8/anotify.egg-info/PKG-INFO` & `anotify-0.0.9/anotify.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anotify
-Version: 0.0.8
+Version: 0.0.9
 Summary: Send notifications by multiple channels.
 Home-page: https://github.com/TommyMerlin/ANotify
 Author: 7ommy
 Author-email: tommymerlin0920@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -33,14 +33,22 @@
 AgentId = ''
 
 wn = Nwecom.WxNotify(corpid=CORPID, corpsecret=CORPSECRET, agentid=AgentId)
 wn.send_msg("test message")
 wn.send_text_card("test title", "test content", "https://www.example.com")
 wn.send_file("./test.txt")
 wn.send_img("./test.png")
+
+# Webhook
+WEB_HOOK = "https://qyapi.weixin.qq.com/cgi-bin/webhook/send?key=xxxxxx"
+wn_webhook = Nwecom.WxWebhookNotify(WEB_HOOK)
+wn_webhook.send_msg("Hello")
+wn_webhook.send_msg_markdown("**Hello**\n- test1\n- [ANotify](https://github.com/TommyMerlin/ANotify)")
+wn_webhook.send_img("E:/Desktop/gpt/Cursor_Demo/test.png")
+wn_webhook.send_file("test.png")
 ```
 
 ### 飞书
 [官网](https://open.feishu.cn/document/server-docs/im-v1/introduction)  
 [创建应用](https://open.feishu.cn/document/home/introduction-to-custom-app-development/self-built-application-development-process)  
 [API调试台](https://open.feishu.cn/api-explorer?from=op_doc_tab)  
 [获取消息发送对象 openid](https://open.feishu.cn/document/faq/trouble-shooting/how-to-obtain-openid)
```

#### html2text {}

```diff
@@ -1,21 +1,26 @@
-Metadata-Version: 2.1 Name: anotify Version: 0.0.8 Summary: Send notifications
+Metadata-Version: 2.1 Name: anotify Version: 0.0.9 Summary: Send notifications
 by multiple channels. Home-page: https://github.com/TommyMerlin/ANotify Author:
 7ommy Author-email: tommymerlin0920@gmail.com License: MIT Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Requires-Python: >=3.6 Description-Content-Type: text/markdown License-
 File: LICENSE Requires-Dist: requests>=2.15.1 ![Alt](https://
 repobeats.axiom.co/api/embed/e1ca45165d69b8370c78d60260a6474b49621fac.svg
 "Repobeats analytics image") ## å®è£ ```console pip install anotify ``` ##
 å®ä¾ ### ä¼ä¸å¾®ä¿¡ [å®ç½](https://work.weixin.qq.com/) ```python from
 ANotify import Nwecom # ä¼ä¸ID CORPID = '' # åºç¨Secret CORPSECRET = '' #
 åºç¨ID AgentId = '' wn = Nwecom.WxNotify(corpid=CORPID,
 corpsecret=CORPSECRET, agentid=AgentId) wn.send_msg("test message")
 wn.send_text_card("test title", "test content", "https://www.example.com")
-wn.send_file("./test.txt") wn.send_img("./test.png") ``` ### é£ä¹¦ [å®ç½]
+wn.send_file("./test.txt") wn.send_img("./test.png") # Webhook WEB_HOOK =
+"https://qyapi.weixin.qq.com/cgi-bin/webhook/send?key=xxxxxx" wn_webhook =
+Nwecom.WxWebhookNotify(WEB_HOOK) wn_webhook.send_msg("Hello")
+wn_webhook.send_msg_markdown("**Hello**\n- test1\n- [ANotify](https://
+github.com/TommyMerlin/ANotify)") wn_webhook.send_img("E:/Desktop/gpt/
+Cursor_Demo/test.png") wn_webhook.send_file("test.png") ``` ### é£ä¹¦ [å®ç½]
 (https://open.feishu.cn/document/server-docs/im-v1/introduction) [åå»ºåºç¨]
 (https://open.feishu.cn/document/home/introduction-to-custom-app-development/
 self-built-application-development-process) [APIè°è¯å°](https://
 open.feishu.cn/api-explorer?from=op_doc_tab) [è·åæ¶æ¯åéå¯¹è±¡ openid]
 (https://open.feishu.cn/document/faq/trouble-shooting/how-to-obtain-openid)
 [Webhookè¯·æ±åéæ¶æ¯](https://open.feishu.cn/document/client-docs/bot-v3/
 add-custom-bot#355ec8c0) ```python from ANotify import Nfeishu APPID = ''
```

### Comparing `anotify-0.0.8/setup.py` & `anotify-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='anotify',
-    version='0.0.8',
+    version='0.0.9',
     packages=find_packages(),
     install_requires=[
         'requests>=2.15.1',
     ],
     author='7ommy',
     author_email='tommymerlin0920@gmail.com',
     description='Send notifications by multiple channels.',
```

