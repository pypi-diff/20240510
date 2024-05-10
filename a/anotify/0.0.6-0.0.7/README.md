# Comparing `tmp/anotify-0.0.6.tar.gz` & `tmp/anotify-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anotify-0.0.6.tar", last modified: Wed May  8 11:55:43 2024, max compression
+gzip compressed data, was "anotify-0.0.7.tar", last modified: Fri May 10 04:15:03 2024, max compression
```

## Comparing `anotify-0.0.6.tar` & `anotify-0.0.7.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 11:55:43.277716 anotify-0.0.6/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 11:55:43.277716 anotify-0.0.6/ANotify/
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-05-08 11:55:38.000000 anotify-0.0.6/ANotify/Nanpush.py
--rw-r--r--   0 runner    (1001) docker     (127)     2643 2024-05-08 11:55:38.000000 anotify-0.0.6/ANotify/Nemail.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-08 11:55:38.000000 anotify-0.0.6/ANotify/Niyuu.py
--rw-r--r--   0 runner    (1001) docker     (127)     1567 2024-05-08 11:55:38.000000 anotify-0.0.6/ANotify/Npushplus.py
--rw-r--r--   0 runner    (1001) docker     (127)      720 2024-05-08 11:55:38.000000 anotify-0.0.6/ANotify/Nserverchan.py
--rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-05-08 11:55:38.000000 anotify-0.0.6/ANotify/Ntelegram.py
--rw-r--r--   0 runner    (1001) docker     (127)     6128 2024-05-08 11:55:38.000000 anotify-0.0.6/ANotify/Nwecom.py
--rw-r--r--   0 runner    (1001) docker     (127)      850 2024-05-08 11:55:38.000000 anotify-0.0.6/ANotify/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-08 11:55:38.000000 anotify-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3470 2024-05-08 11:55:43.277716 anotify-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3035 2024-05-08 11:55:38.000000 anotify-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 11:55:43.277716 anotify-0.0.6/anotify.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3470 2024-05-08 11:55:43.000000 anotify-0.0.6/anotify.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-08 11:55:43.000000 anotify-0.0.6/anotify.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 11:55:43.000000 anotify-0.0.6/anotify.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-08 11:55:43.000000 anotify-0.0.6/anotify.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-08 11:55:43.000000 anotify-0.0.6/anotify.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 11:55:43.277716 anotify-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-05-08 11:55:38.000000 anotify-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 04:15:03.104667 anotify-0.0.7/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 04:15:03.104667 anotify-0.0.7/ANotify/
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-05-10 04:14:58.000000 anotify-0.0.7/ANotify/Nanpush.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2643 2024-05-10 04:14:58.000000 anotify-0.0.7/ANotify/Nemail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2662 2024-05-10 04:14:58.000000 anotify-0.0.7/ANotify/Nfeishu.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-10 04:14:58.000000 anotify-0.0.7/ANotify/Niyuu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1567 2024-05-10 04:14:58.000000 anotify-0.0.7/ANotify/Npushplus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-05-10 04:14:58.000000 anotify-0.0.7/ANotify/Nserverchan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-05-10 04:14:58.000000 anotify-0.0.7/ANotify/Ntelegram.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6128 2024-05-10 04:14:58.000000 anotify-0.0.7/ANotify/Nwecom.py
+-rw-r--r--   0 runner    (1001) docker     (127)      850 2024-05-10 04:14:58.000000 anotify-0.0.7/ANotify/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-10 04:14:58.000000 anotify-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4525 2024-05-10 04:15:03.104667 anotify-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4090 2024-05-10 04:14:58.000000 anotify-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 04:15:03.104667 anotify-0.0.7/anotify.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4525 2024-05-10 04:15:03.000000 anotify-0.0.7/anotify.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-05-10 04:15:03.000000 anotify-0.0.7/anotify.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 04:15:03.000000 anotify-0.0.7/anotify.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-10 04:15:03.000000 anotify-0.0.7/anotify.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-10 04:15:03.000000 anotify-0.0.7/anotify.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 04:15:03.104667 anotify-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-05-10 04:14:58.000000 anotify-0.0.7/setup.py
```

### Comparing `anotify-0.0.6/ANotify/Nanpush.py` & `anotify-0.0.7/ANotify/Nanpush.py`

 * *Files identical despite different names*

### Comparing `anotify-0.0.6/ANotify/Nemail.py` & `anotify-0.0.7/ANotify/Nemail.py`

 * *Files identical despite different names*

### Comparing `anotify-0.0.6/ANotify/Npushplus.py` & `anotify-0.0.7/ANotify/Npushplus.py`

 * *Files identical despite different names*

### Comparing `anotify-0.0.6/ANotify/Nserverchan.py` & `anotify-0.0.7/ANotify/Nserverchan.py`

 * *Files identical despite different names*

### Comparing `anotify-0.0.6/ANotify/Ntelegram.py` & `anotify-0.0.7/ANotify/Ntelegram.py`

 * *Files identical despite different names*

### Comparing `anotify-0.0.6/ANotify/Nwecom.py` & `anotify-0.0.7/ANotify/Nwecom.py`

 * *Files identical despite different names*

### Comparing `anotify-0.0.6/ANotify/__init__.py` & `anotify-0.0.7/ANotify/__init__.py`

 * *Files identical despite different names*

### Comparing `anotify-0.0.6/LICENSE` & `anotify-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `anotify-0.0.6/PKG-INFO` & `anotify-0.0.7/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anotify
-Version: 0.0.6
+Version: 0.0.7
 Summary: Send notifications by multiple channels.
 Home-page: https://github.com/TommyMerlin/ANotify
 Author: 7ommy
 Author-email: tommymerlin0920@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -35,14 +35,41 @@
 wn = Nwecom.WxNotify(corpid=CORPID, corpsecret=CORPSECRET, agentid=AgentId)
 wn.send_msg("test message")
 wn.send_text_card("test title", "test content", "https://www.example.com")
 wn.send_file("./test.txt")
 wn.send_img("./test.png")
 ```
 
+### 飞书
+[官网](https://open.feishu.cn/document/server-docs/im-v1/introduction)  
+[创建应用](https://open.feishu.cn/document/home/introduction-to-custom-app-development/self-built-application-development-process)  
+[API调试台](https://open.feishu.cn/api-explorer?from=op_doc_tab)  
+[获取消息发送对象 openid](https://open.feishu.cn/document/faq/trouble-shooting/how-to-obtain-openid)  
+[Webhook请求发送消息](https://open.feishu.cn/document/client-docs/bot-v3/add-custom-bot#355ec8c0)
+```python
+from ANotify import Nfeishu
+APPID = ''
+APPSECRET = ''
+OPEN_ID = ''
+UNION_ID = ''
+USER_ID = ''
+CHAT_ID = ''
+
+feishu = Nfeishu.FeishuNotify(appid=APPID, appsecret=APPSECRET)
+feishu.send_msg(Nfeishu.ReceiverType.OPEN_ID, OPEN_ID, "Hello World!")
+feishu.send_msg(Nfeishu.ReceiverType.UINION_ID, UNION_ID, "Hello World!")
+feishu.send_msg(Nfeishu.ReceiverType.USER_ID, USER_ID, "Hello World!")
+feishu.send_msg(Nfeishu.ReceiverType.CHAT_ID, CHAT_ID, "Hello World!")
+
+# Webhook
+feishu_webhook = Nfeishu.FeishuWebhookNotify("https://open.feishu.cn/open-apis/bot/v2/hook/xxxxxx")
+feishu_webhook.send_msg("Hello World!")
+
+```
+
 ### AnPush
 [官网](https://anpush.com/)
 ```python
 from ANotify import Nanpush
 TOKEN = ""
 anpush = Nanpush.AnpushNotify(TOKEN)
 anpush.send_msg("title", "content", "channel_id")
@@ -114,12 +141,9 @@
 MAIL_USER = ''
 # 密码(部分邮箱为授权码)
 MAIL_PASS = ''
 # 邮件发送方邮箱地址
 SENDER = ''
 
 email_notify = Nemail.EmailNotify(MAIL_HOST, MAIL_USER, MAIL_PASS, SENDER)
-if email_notify.send_email("测试标题", "测试正文", attachment_filename=None, receiver='123@example.com'):
-    print("邮件发送成功√")
-else:
-    print("邮件发送失败×")
+email_notify.send_email("测试标题", "测试正文", attachment_filename=None, receiver='123@example.com')
 ```
```

#### html2text {}

```diff
@@ -1,28 +1,43 @@
-Metadata-Version: 2.1 Name: anotify Version: 0.0.6 Summary: Send notifications
+Metadata-Version: 2.1 Name: anotify Version: 0.0.7 Summary: Send notifications
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
-wn.send_file("./test.txt") wn.send_img("./test.png") ``` ### AnPush [å®ç½]
-(https://anpush.com/) ```python from ANotify import Nanpush TOKEN = "" anpush =
-Nanpush.AnpushNotify(TOKEN) anpush.send_msg("title", "content", "channel_id")
-``` ### IYUU [å®ç½](https://iyuu.cn/) ```python from ANotify import Niyuu
-TOKEN = "" iyuu = Niyuu.IyuuNotify(TOKEN) iyuu.send_msg("title", "content") ```
-### PushPlus [å®ç½](https://www.pushplus.plus/) ```python from ANotify import
-NPushPlus TOKEN = '' pushplus = Npushplus.PushPlusNotify(TOKEN) pushplus =
-Npushplus.PushPlusNotify(TOKEN) pushplus.send_msg("æµè¯æ é¢",
+wn.send_file("./test.txt") wn.send_img("./test.png") ``` ### é£ä¹¦ [å®ç½]
+(https://open.feishu.cn/document/server-docs/im-v1/introduction) [åå»ºåºç¨]
+(https://open.feishu.cn/document/home/introduction-to-custom-app-development/
+self-built-application-development-process) [APIè°è¯å°](https://
+open.feishu.cn/api-explorer?from=op_doc_tab) [è·åæ¶æ¯åéå¯¹è±¡ openid]
+(https://open.feishu.cn/document/faq/trouble-shooting/how-to-obtain-openid)
+[Webhookè¯·æ±åéæ¶æ¯](https://open.feishu.cn/document/client-docs/bot-v3/
+add-custom-bot#355ec8c0) ```python from ANotify import Nfeishu APPID = ''
+APPSECRET = '' OPEN_ID = '' UNION_ID = '' USER_ID = '' CHAT_ID = '' feishu =
+Nfeishu.FeishuNotify(appid=APPID, appsecret=APPSECRET) feishu.send_msg
+(Nfeishu.ReceiverType.OPEN_ID, OPEN_ID, "Hello World!") feishu.send_msg
+(Nfeishu.ReceiverType.UINION_ID, UNION_ID, "Hello World!") feishu.send_msg
+(Nfeishu.ReceiverType.USER_ID, USER_ID, "Hello World!") feishu.send_msg
+(Nfeishu.ReceiverType.CHAT_ID, CHAT_ID, "Hello World!") # Webhook
+feishu_webhook = Nfeishu.FeishuWebhookNotify("https://open.feishu.cn/open-apis/
+bot/v2/hook/xxxxxx") feishu_webhook.send_msg("Hello World!") ``` ### AnPush
+[å®ç½](https://anpush.com/) ```python from ANotify import Nanpush TOKEN = ""
+anpush = Nanpush.AnpushNotify(TOKEN) anpush.send_msg("title", "content",
+"channel_id") ``` ### IYUU [å®ç½](https://iyuu.cn/) ```python from ANotify
+import Niyuu TOKEN = "" iyuu = Niyuu.IyuuNotify(TOKEN) iyuu.send_msg("title",
+"content") ``` ### PushPlus [å®ç½](https://www.pushplus.plus/) ```python from
+ANotify import NPushPlus TOKEN = '' pushplus = Npushplus.PushPlusNotify(TOKEN)
+pushplus = Npushplus.PushPlusNotify(TOKEN) pushplus.send_msg("æµè¯æ é¢",
 "æµè¯æ­£æ", Npushplus.TemplateType.txt) msg_json = { "status": 200, "msg":
 "success" } pushplus.send_msg("æµè¯æ é¢", msg_json,
 Npushplus.TemplateType.json) pushplus.send_msg("æµè¯æ é¢",
 "**æµè¯åå®¹**\n- test1\n- [ANotify](https://github.com/TommyMerlin/
 ANotify)", Npushplus.TemplateType.markdown) pushplus.send_msg("æµè¯æ é¢",
 "æµè¯åå®¹_A_N_o_t_i_f_y", Npushplus.TemplateType.html) ``` ### Serveré± [å®ç½]
 (https://sct.ftqq.com/) ```python from ANotify import Nserverchan TOKEN = ''
@@ -36,11 +51,10 @@
 message", Ntelegram.ParseMode.TEXT, proxy=proxy) # æä»£ç telegram.send_msg
 ("[link](https://www.example.com)", Ntelegram.ParseMode.Markdown)
 telegram.send_msg("_l_i_n_k", Ntelegram.ParseMode.HTML) telegram.send_photo
 ("test.png","test") telegram.send_file("test.txt", "test") ``` ### Email
 ```python from ANotify import Nemail # é®ç®±æå¡å¨å°å MAIL_HOST = '' #
 ç¨æ·å MAIL_USER = '' # å¯ç (é¨åé®ç®±ä¸ºææç ) MAIL_PASS = '' #
 é®ä»¶åéæ¹é®ç®±å°å SENDER = '' email_notify = Nemail.EmailNotify
-(MAIL_HOST, MAIL_USER, MAIL_PASS, SENDER) if email_notify.send_email
+(MAIL_HOST, MAIL_USER, MAIL_PASS, SENDER) email_notify.send_email
 ("æµè¯æ é¢", "æµè¯æ­£æ", attachment_filename=None,
-receiver='123@example.com'): print("é®ä»¶åéæåâ") else: print
-("é®ä»¶åéå¤±è´¥Ã") ```
+receiver='123@example.com') ```
```

### Comparing `anotify-0.0.6/README.md` & `anotify-0.0.7/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -20,14 +20,41 @@
 wn = Nwecom.WxNotify(corpid=CORPID, corpsecret=CORPSECRET, agentid=AgentId)
 wn.send_msg("test message")
 wn.send_text_card("test title", "test content", "https://www.example.com")
 wn.send_file("./test.txt")
 wn.send_img("./test.png")
 ```
 
+### 飞书
+[官网](https://open.feishu.cn/document/server-docs/im-v1/introduction)  
+[创建应用](https://open.feishu.cn/document/home/introduction-to-custom-app-development/self-built-application-development-process)  
+[API调试台](https://open.feishu.cn/api-explorer?from=op_doc_tab)  
+[获取消息发送对象 openid](https://open.feishu.cn/document/faq/trouble-shooting/how-to-obtain-openid)  
+[Webhook请求发送消息](https://open.feishu.cn/document/client-docs/bot-v3/add-custom-bot#355ec8c0)
+```python
+from ANotify import Nfeishu
+APPID = ''
+APPSECRET = ''
+OPEN_ID = ''
+UNION_ID = ''
+USER_ID = ''
+CHAT_ID = ''
+
+feishu = Nfeishu.FeishuNotify(appid=APPID, appsecret=APPSECRET)
+feishu.send_msg(Nfeishu.ReceiverType.OPEN_ID, OPEN_ID, "Hello World!")
+feishu.send_msg(Nfeishu.ReceiverType.UINION_ID, UNION_ID, "Hello World!")
+feishu.send_msg(Nfeishu.ReceiverType.USER_ID, USER_ID, "Hello World!")
+feishu.send_msg(Nfeishu.ReceiverType.CHAT_ID, CHAT_ID, "Hello World!")
+
+# Webhook
+feishu_webhook = Nfeishu.FeishuWebhookNotify("https://open.feishu.cn/open-apis/bot/v2/hook/xxxxxx")
+feishu_webhook.send_msg("Hello World!")
+
+```
+
 ### AnPush
 [官网](https://anpush.com/)
 ```python
 from ANotify import Nanpush
 TOKEN = ""
 anpush = Nanpush.AnpushNotify(TOKEN)
 anpush.send_msg("title", "content", "channel_id")
@@ -99,12 +126,9 @@
 MAIL_USER = ''
 # 密码(部分邮箱为授权码)
 MAIL_PASS = ''
 # 邮件发送方邮箱地址
 SENDER = ''
 
 email_notify = Nemail.EmailNotify(MAIL_HOST, MAIL_USER, MAIL_PASS, SENDER)
-if email_notify.send_email("测试标题", "测试正文", attachment_filename=None, receiver='123@example.com'):
-    print("邮件发送成功√")
-else:
-    print("邮件发送失败×")
+email_notify.send_email("测试标题", "测试正文", attachment_filename=None, receiver='123@example.com')
 ```
```

#### html2text {}

```diff
@@ -2,21 +2,36 @@
 e1ca45165d69b8370c78d60260a6474b49621fac.svg "Repobeats analytics image") ##
 å®è£ ```console pip install anotify ``` ## å®ä¾ ### ä¼ä¸å¾®ä¿¡ [å®ç½]
 (https://work.weixin.qq.com/) ```python from ANotify import Nwecom # ä¼ä¸ID
 CORPID = '' # åºç¨Secret CORPSECRET = '' # åºç¨ID AgentId = '' wn =
 Nwecom.WxNotify(corpid=CORPID, corpsecret=CORPSECRET, agentid=AgentId)
 wn.send_msg("test message") wn.send_text_card("test title", "test content",
 "https://www.example.com") wn.send_file("./test.txt") wn.send_img("./test.png")
-``` ### AnPush [å®ç½](https://anpush.com/) ```python from ANotify import
-Nanpush TOKEN = "" anpush = Nanpush.AnpushNotify(TOKEN) anpush.send_msg
-("title", "content", "channel_id") ``` ### IYUU [å®ç½](https://iyuu.cn/
-) ```python from ANotify import Niyuu TOKEN = "" iyuu = Niyuu.IyuuNotify(TOKEN)
-iyuu.send_msg("title", "content") ``` ### PushPlus [å®ç½](https://
-www.pushplus.plus/) ```python from ANotify import NPushPlus TOKEN = '' pushplus
-= Npushplus.PushPlusNotify(TOKEN) pushplus = Npushplus.PushPlusNotify(TOKEN)
+``` ### é£ä¹¦ [å®ç½](https://open.feishu.cn/document/server-docs/im-v1/
+introduction) [åå»ºåºç¨](https://open.feishu.cn/document/home/introduction-
+to-custom-app-development/self-built-application-development-process)
+[APIè°è¯å°](https://open.feishu.cn/api-explorer?from=op_doc_tab)
+[è·åæ¶æ¯åéå¯¹è±¡ openid](https://open.feishu.cn/document/faq/trouble-
+shooting/how-to-obtain-openid) [Webhookè¯·æ±åéæ¶æ¯](https://
+open.feishu.cn/document/client-docs/bot-v3/add-custom-bot#355ec8c0) ```python
+from ANotify import Nfeishu APPID = '' APPSECRET = '' OPEN_ID = '' UNION_ID =
+'' USER_ID = '' CHAT_ID = '' feishu = Nfeishu.FeishuNotify(appid=APPID,
+appsecret=APPSECRET) feishu.send_msg(Nfeishu.ReceiverType.OPEN_ID, OPEN_ID,
+"Hello World!") feishu.send_msg(Nfeishu.ReceiverType.UINION_ID, UNION_ID,
+"Hello World!") feishu.send_msg(Nfeishu.ReceiverType.USER_ID, USER_ID, "Hello
+World!") feishu.send_msg(Nfeishu.ReceiverType.CHAT_ID, CHAT_ID, "Hello World!")
+# Webhook feishu_webhook = Nfeishu.FeishuWebhookNotify("https://open.feishu.cn/
+open-apis/bot/v2/hook/xxxxxx") feishu_webhook.send_msg("Hello World!") ``` ###
+AnPush [å®ç½](https://anpush.com/) ```python from ANotify import Nanpush
+TOKEN = "" anpush = Nanpush.AnpushNotify(TOKEN) anpush.send_msg("title",
+"content", "channel_id") ``` ### IYUU [å®ç½](https://iyuu.cn/) ```python from
+ANotify import Niyuu TOKEN = "" iyuu = Niyuu.IyuuNotify(TOKEN) iyuu.send_msg
+("title", "content") ``` ### PushPlus [å®ç½](https://www.pushplus.plus/
+) ```python from ANotify import NPushPlus TOKEN = '' pushplus =
+Npushplus.PushPlusNotify(TOKEN) pushplus = Npushplus.PushPlusNotify(TOKEN)
 pushplus.send_msg("æµè¯æ é¢", "æµè¯æ­£æ", Npushplus.TemplateType.txt)
 msg_json = { "status": 200, "msg": "success" } pushplus.send_msg
 ("æµè¯æ é¢", msg_json, Npushplus.TemplateType.json) pushplus.send_msg
 ("æµè¯æ é¢", "**æµè¯åå®¹**\n- test1\n- [ANotify](https://github.com/
 TommyMerlin/ANotify)", Npushplus.TemplateType.markdown) pushplus.send_msg
 ("æµè¯æ é¢", "æµè¯åå®¹_A_N_o_t_i_f_y", Npushplus.TemplateType.html) ``` ###
 Serveré± [å®ç½](https://sct.ftqq.com/) ```python from ANotify import
@@ -31,10 +46,9 @@
 Ntelegram.ParseMode.TEXT, proxy=proxy) # æä»£ç telegram.send_msg("[link]
 (https://www.example.com)", Ntelegram.ParseMode.Markdown) telegram.send_msg
 ("_l_i_n_k", Ntelegram.ParseMode.HTML) telegram.send_photo("test.png","test")
 telegram.send_file("test.txt", "test") ``` ### Email ```python from ANotify
 import Nemail # é®ç®±æå¡å¨å°å MAIL_HOST = '' # ç¨æ·å MAIL_USER = ''
 # å¯ç (é¨åé®ç®±ä¸ºææç ) MAIL_PASS = '' # é®ä»¶åéæ¹é®ç®±å°å
 SENDER = '' email_notify = Nemail.EmailNotify(MAIL_HOST, MAIL_USER, MAIL_PASS,
-SENDER) if email_notify.send_email("æµè¯æ é¢", "æµè¯æ­£æ",
-attachment_filename=None, receiver='123@example.com'): print
-("é®ä»¶åéæåâ") else: print("é®ä»¶åéå¤±è´¥Ã") ```
+SENDER) email_notify.send_email("æµè¯æ é¢", "æµè¯æ­£æ",
+attachment_filename=None, receiver='123@example.com') ```
```

### Comparing `anotify-0.0.6/anotify.egg-info/PKG-INFO` & `anotify-0.0.7/anotify.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anotify
-Version: 0.0.6
+Version: 0.0.7
 Summary: Send notifications by multiple channels.
 Home-page: https://github.com/TommyMerlin/ANotify
 Author: 7ommy
 Author-email: tommymerlin0920@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -35,14 +35,41 @@
 wn = Nwecom.WxNotify(corpid=CORPID, corpsecret=CORPSECRET, agentid=AgentId)
 wn.send_msg("test message")
 wn.send_text_card("test title", "test content", "https://www.example.com")
 wn.send_file("./test.txt")
 wn.send_img("./test.png")
 ```
 
+### 飞书
+[官网](https://open.feishu.cn/document/server-docs/im-v1/introduction)  
+[创建应用](https://open.feishu.cn/document/home/introduction-to-custom-app-development/self-built-application-development-process)  
+[API调试台](https://open.feishu.cn/api-explorer?from=op_doc_tab)  
+[获取消息发送对象 openid](https://open.feishu.cn/document/faq/trouble-shooting/how-to-obtain-openid)  
+[Webhook请求发送消息](https://open.feishu.cn/document/client-docs/bot-v3/add-custom-bot#355ec8c0)
+```python
+from ANotify import Nfeishu
+APPID = ''
+APPSECRET = ''
+OPEN_ID = ''
+UNION_ID = ''
+USER_ID = ''
+CHAT_ID = ''
+
+feishu = Nfeishu.FeishuNotify(appid=APPID, appsecret=APPSECRET)
+feishu.send_msg(Nfeishu.ReceiverType.OPEN_ID, OPEN_ID, "Hello World!")
+feishu.send_msg(Nfeishu.ReceiverType.UINION_ID, UNION_ID, "Hello World!")
+feishu.send_msg(Nfeishu.ReceiverType.USER_ID, USER_ID, "Hello World!")
+feishu.send_msg(Nfeishu.ReceiverType.CHAT_ID, CHAT_ID, "Hello World!")
+
+# Webhook
+feishu_webhook = Nfeishu.FeishuWebhookNotify("https://open.feishu.cn/open-apis/bot/v2/hook/xxxxxx")
+feishu_webhook.send_msg("Hello World!")
+
+```
+
 ### AnPush
 [官网](https://anpush.com/)
 ```python
 from ANotify import Nanpush
 TOKEN = ""
 anpush = Nanpush.AnpushNotify(TOKEN)
 anpush.send_msg("title", "content", "channel_id")
@@ -114,12 +141,9 @@
 MAIL_USER = ''
 # 密码(部分邮箱为授权码)
 MAIL_PASS = ''
 # 邮件发送方邮箱地址
 SENDER = ''
 
 email_notify = Nemail.EmailNotify(MAIL_HOST, MAIL_USER, MAIL_PASS, SENDER)
-if email_notify.send_email("测试标题", "测试正文", attachment_filename=None, receiver='123@example.com'):
-    print("邮件发送成功√")
-else:
-    print("邮件发送失败×")
+email_notify.send_email("测试标题", "测试正文", attachment_filename=None, receiver='123@example.com')
 ```
```

#### html2text {}

```diff
@@ -1,28 +1,43 @@
-Metadata-Version: 2.1 Name: anotify Version: 0.0.6 Summary: Send notifications
+Metadata-Version: 2.1 Name: anotify Version: 0.0.7 Summary: Send notifications
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
-wn.send_file("./test.txt") wn.send_img("./test.png") ``` ### AnPush [å®ç½]
-(https://anpush.com/) ```python from ANotify import Nanpush TOKEN = "" anpush =
-Nanpush.AnpushNotify(TOKEN) anpush.send_msg("title", "content", "channel_id")
-``` ### IYUU [å®ç½](https://iyuu.cn/) ```python from ANotify import Niyuu
-TOKEN = "" iyuu = Niyuu.IyuuNotify(TOKEN) iyuu.send_msg("title", "content") ```
-### PushPlus [å®ç½](https://www.pushplus.plus/) ```python from ANotify import
-NPushPlus TOKEN = '' pushplus = Npushplus.PushPlusNotify(TOKEN) pushplus =
-Npushplus.PushPlusNotify(TOKEN) pushplus.send_msg("æµè¯æ é¢",
+wn.send_file("./test.txt") wn.send_img("./test.png") ``` ### é£ä¹¦ [å®ç½]
+(https://open.feishu.cn/document/server-docs/im-v1/introduction) [åå»ºåºç¨]
+(https://open.feishu.cn/document/home/introduction-to-custom-app-development/
+self-built-application-development-process) [APIè°è¯å°](https://
+open.feishu.cn/api-explorer?from=op_doc_tab) [è·åæ¶æ¯åéå¯¹è±¡ openid]
+(https://open.feishu.cn/document/faq/trouble-shooting/how-to-obtain-openid)
+[Webhookè¯·æ±åéæ¶æ¯](https://open.feishu.cn/document/client-docs/bot-v3/
+add-custom-bot#355ec8c0) ```python from ANotify import Nfeishu APPID = ''
+APPSECRET = '' OPEN_ID = '' UNION_ID = '' USER_ID = '' CHAT_ID = '' feishu =
+Nfeishu.FeishuNotify(appid=APPID, appsecret=APPSECRET) feishu.send_msg
+(Nfeishu.ReceiverType.OPEN_ID, OPEN_ID, "Hello World!") feishu.send_msg
+(Nfeishu.ReceiverType.UINION_ID, UNION_ID, "Hello World!") feishu.send_msg
+(Nfeishu.ReceiverType.USER_ID, USER_ID, "Hello World!") feishu.send_msg
+(Nfeishu.ReceiverType.CHAT_ID, CHAT_ID, "Hello World!") # Webhook
+feishu_webhook = Nfeishu.FeishuWebhookNotify("https://open.feishu.cn/open-apis/
+bot/v2/hook/xxxxxx") feishu_webhook.send_msg("Hello World!") ``` ### AnPush
+[å®ç½](https://anpush.com/) ```python from ANotify import Nanpush TOKEN = ""
+anpush = Nanpush.AnpushNotify(TOKEN) anpush.send_msg("title", "content",
+"channel_id") ``` ### IYUU [å®ç½](https://iyuu.cn/) ```python from ANotify
+import Niyuu TOKEN = "" iyuu = Niyuu.IyuuNotify(TOKEN) iyuu.send_msg("title",
+"content") ``` ### PushPlus [å®ç½](https://www.pushplus.plus/) ```python from
+ANotify import NPushPlus TOKEN = '' pushplus = Npushplus.PushPlusNotify(TOKEN)
+pushplus = Npushplus.PushPlusNotify(TOKEN) pushplus.send_msg("æµè¯æ é¢",
 "æµè¯æ­£æ", Npushplus.TemplateType.txt) msg_json = { "status": 200, "msg":
 "success" } pushplus.send_msg("æµè¯æ é¢", msg_json,
 Npushplus.TemplateType.json) pushplus.send_msg("æµè¯æ é¢",
 "**æµè¯åå®¹**\n- test1\n- [ANotify](https://github.com/TommyMerlin/
 ANotify)", Npushplus.TemplateType.markdown) pushplus.send_msg("æµè¯æ é¢",
 "æµè¯åå®¹_A_N_o_t_i_f_y", Npushplus.TemplateType.html) ``` ### Serveré± [å®ç½]
 (https://sct.ftqq.com/) ```python from ANotify import Nserverchan TOKEN = ''
@@ -36,11 +51,10 @@
 message", Ntelegram.ParseMode.TEXT, proxy=proxy) # æä»£ç telegram.send_msg
 ("[link](https://www.example.com)", Ntelegram.ParseMode.Markdown)
 telegram.send_msg("_l_i_n_k", Ntelegram.ParseMode.HTML) telegram.send_photo
 ("test.png","test") telegram.send_file("test.txt", "test") ``` ### Email
 ```python from ANotify import Nemail # é®ç®±æå¡å¨å°å MAIL_HOST = '' #
 ç¨æ·å MAIL_USER = '' # å¯ç (é¨åé®ç®±ä¸ºææç ) MAIL_PASS = '' #
 é®ä»¶åéæ¹é®ç®±å°å SENDER = '' email_notify = Nemail.EmailNotify
-(MAIL_HOST, MAIL_USER, MAIL_PASS, SENDER) if email_notify.send_email
+(MAIL_HOST, MAIL_USER, MAIL_PASS, SENDER) email_notify.send_email
 ("æµè¯æ é¢", "æµè¯æ­£æ", attachment_filename=None,
-receiver='123@example.com'): print("é®ä»¶åéæåâ") else: print
-("é®ä»¶åéå¤±è´¥Ã") ```
+receiver='123@example.com') ```
```

### Comparing `anotify-0.0.6/setup.py` & `anotify-0.0.7/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='anotify',
-    version='0.0.6',
+    version='0.0.7',
     packages=find_packages(),
     install_requires=[
         'requests>=2.15.1',
     ],
     author='7ommy',
     author_email='tommymerlin0920@gmail.com',
     description='Send notifications by multiple channels.',
```

