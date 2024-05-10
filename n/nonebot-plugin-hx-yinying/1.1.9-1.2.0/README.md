# Comparing `tmp/nonebot-plugin-hx-yinying-1.1.9.tar.gz` & `tmp/nonebot-plugin-hx-yinying-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-hx-yinying-1.1.9.tar", last modified: Thu May  9 13:49:53 2024, max compression
+gzip compressed data, was "nonebot-plugin-hx-yinying-1.2.0.tar", last modified: Fri May 10 17:56:18 2024, max compression
```

## Comparing `nonebot-plugin-hx-yinying-1.1.9.tar` & `nonebot-plugin-hx-yinying-1.2.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-05-09 13:49:53.429334 nonebot-plugin-hx-yinying-1.1.9/
--rw-rw-rw-   0        0        0     1098 2024-04-16 15:27:11.000000 nonebot-plugin-hx-yinying-1.1.9/LICENSE
--rw-rw-rw-   0        0        0     6502 2024-05-09 13:49:53.431345 nonebot-plugin-hx-yinying-1.1.9/PKG-INFO
--rw-rw-rw-   0        0        0     6062 2024-04-28 16:24:12.000000 nonebot-plugin-hx-yinying-1.1.9/README.md
-drwxrwxrwx   0        0        0        0 2024-05-09 13:49:53.278651 nonebot-plugin-hx-yinying-1.1.9/nonebot_plugin_hx_yinying/
--rw-rw-rw-   0        0        0    57847 2024-05-07 15:39:33.000000 nonebot-plugin-hx-yinying-1.1.9/nonebot_plugin_hx_yinying/__init__.py
--rw-rw-rw-   0        0        0    91003 2024-05-08 16:28:38.000000 nonebot-plugin-hx-yinying-1.1.9/nonebot_plugin_hx_yinying/chat.py
--rw-rw-rw-   0        0        0     1532 2024-05-09 13:49:42.000000 nonebot-plugin-hx-yinying-1.1.9/nonebot_plugin_hx_yinying/config.py
--rw-rw-rw-   0        0        0     2364 2024-05-06 19:18:29.000000 nonebot-plugin-hx-yinying-1.1.9/nonebot_plugin_hx_yinying/image_check.py
--rw-rw-rw-   0        0        0     5501 2024-05-09 13:48:28.000000 nonebot-plugin-hx-yinying-1.1.9/nonebot_plugin_hx_yinying/report.py
--rw-rw-rw-   0        0        0     5038 2024-04-28 10:07:11.000000 nonebot-plugin-hx-yinying-1.1.9/nonebot_plugin_hx_yinying/smms.py
-drwxrwxrwx   0        0        0        0 2024-05-09 13:49:53.424330 nonebot-plugin-hx-yinying-1.1.9/nonebot_plugin_hx_yinying.egg-info/
--rw-rw-rw-   0        0        0     6502 2024-05-09 13:49:52.000000 nonebot-plugin-hx-yinying-1.1.9/nonebot_plugin_hx_yinying.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      499 2024-05-09 13:49:52.000000 nonebot-plugin-hx-yinying-1.1.9/nonebot_plugin_hx_yinying.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-09 13:49:52.000000 nonebot-plugin-hx-yinying-1.1.9/nonebot_plugin_hx_yinying.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      274 2024-05-09 13:49:52.000000 nonebot-plugin-hx-yinying-1.1.9/nonebot_plugin_hx_yinying.egg-info/requires.txt
--rw-rw-rw-   0        0        0       26 2024-05-09 13:49:52.000000 nonebot-plugin-hx-yinying-1.1.9/nonebot_plugin_hx_yinying.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       85 2024-05-09 13:49:53.439854 nonebot-plugin-hx-yinying-1.1.9/setup.cfg
--rw-rw-rw-   0        0        0     1002 2024-05-09 13:49:49.000000 nonebot-plugin-hx-yinying-1.1.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-10 17:56:18.662410 nonebot-plugin-hx-yinying-1.2.0/
+-rw-rw-rw-   0        0        0     1098 2024-04-16 15:27:11.000000 nonebot-plugin-hx-yinying-1.2.0/LICENSE
+-rw-rw-rw-   0        0        0     6502 2024-05-10 17:56:18.666539 nonebot-plugin-hx-yinying-1.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     6062 2024-04-28 16:24:12.000000 nonebot-plugin-hx-yinying-1.2.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-10 17:56:18.518412 nonebot-plugin-hx-yinying-1.2.0/nonebot_plugin_hx_yinying/
+-rw-rw-rw-   0        0        0    57847 2024-05-07 15:39:33.000000 nonebot-plugin-hx-yinying-1.2.0/nonebot_plugin_hx_yinying/__init__.py
+-rw-rw-rw-   0        0        0    91238 2024-05-10 16:16:29.000000 nonebot-plugin-hx-yinying-1.2.0/nonebot_plugin_hx_yinying/chat.py
+-rw-rw-rw-   0        0        0     1532 2024-05-10 14:38:31.000000 nonebot-plugin-hx-yinying-1.2.0/nonebot_plugin_hx_yinying/config.py
+-rw-rw-rw-   0        0        0     2553 2024-05-10 15:19:05.000000 nonebot-plugin-hx-yinying-1.2.0/nonebot_plugin_hx_yinying/image_check.py
+-rw-rw-rw-   0        0        0     5501 2024-05-09 13:48:28.000000 nonebot-plugin-hx-yinying-1.2.0/nonebot_plugin_hx_yinying/report.py
+-rw-rw-rw-   0        0        0     5038 2024-05-10 14:31:14.000000 nonebot-plugin-hx-yinying-1.2.0/nonebot_plugin_hx_yinying/smms.py
+drwxrwxrwx   0        0        0        0 2024-05-10 17:56:18.657411 nonebot-plugin-hx-yinying-1.2.0/nonebot_plugin_hx_yinying.egg-info/
+-rw-rw-rw-   0        0        0     6502 2024-05-10 17:56:17.000000 nonebot-plugin-hx-yinying-1.2.0/nonebot_plugin_hx_yinying.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      499 2024-05-10 17:56:18.000000 nonebot-plugin-hx-yinying-1.2.0/nonebot_plugin_hx_yinying.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-10 17:56:17.000000 nonebot-plugin-hx-yinying-1.2.0/nonebot_plugin_hx_yinying.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      274 2024-05-10 17:56:17.000000 nonebot-plugin-hx-yinying-1.2.0/nonebot_plugin_hx_yinying.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       26 2024-05-10 17:56:17.000000 nonebot-plugin-hx-yinying-1.2.0/nonebot_plugin_hx_yinying.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       85 2024-05-10 17:56:18.677973 nonebot-plugin-hx-yinying-1.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1002 2024-05-10 17:56:00.000000 nonebot-plugin-hx-yinying-1.2.0/setup.py
```

### Comparing `nonebot-plugin-hx-yinying-1.1.9/LICENSE` & `nonebot-plugin-hx-yinying-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-hx-yinying-1.1.9/PKG-INFO` & `nonebot-plugin-hx-yinying-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-hx-yinying
-Version: 1.1.9
+Version: 1.2.0
 Summary: chat with yinying
 Home-page: https://github.com/huanxin996/nonebot_plugin_hx-yinying
 Author: Huan Xin
 Author-email: mc.xiaolang@foxmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-hx-yinying Version: 1.1.9 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-hx-yinying Version: 1.2.0 Summary:
 chat with yinying Home-page: https://github.com/huanxin996/nonebot_plugin_hx-
 yinying Author: Huan Xin Author-email: mc.xiaolang@foxmail.com Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Description-Content-
 Type: text/markdown License-File: LICENSE [![All Contributors](https://
 img.shields.io/badge/all_contributors-2-orange.svg?style=flat-square)]
 (#contributors-) * @Author : huanxin996 * @Date : 2024-4-17 * @LastEditors :
```

### Comparing `nonebot-plugin-hx-yinying-1.1.9/README.md` & `nonebot-plugin-hx-yinying-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-hx-yinying-1.1.9/nonebot_plugin_hx_yinying/__init__.py` & `nonebot-plugin-hx-yinying-1.2.0/nonebot_plugin_hx_yinying/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-hx-yinying-1.1.9/nonebot_plugin_hx_yinying/chat.py` & `nonebot-plugin-hx-yinying-1.2.0/nonebot_plugin_hx_yinying/chat.py`

 * *Files 2% similar despite different names*

```diff
@@ -997,51 +997,63 @@
         back = False
     return back
 
 #历史消息卡片构建
 async def get_history(id,bot,event) -> List[MessageSegment]:
     date = log_in()
     log_list = date[f"{id}"]["log"]
-    t = len(log_list)/2
+    t = len(log_list)
     nick = await get_nick(bot,event)
     msg_list = []
     try:
         for item in log_list:
             text = item["msg"]
             if item["rule"]=="user":
                 msg_list.append(
                 MessageSegment.node_custom(
                 user_id=id,
-                nickname="呜呜一号",
+                nickname="AAA星佑批发（幻歆限定）",
                 content=Message(f"(来源)[user]\n{text}"),
                 ))
             else:
                 msg_list.append(
                 MessageSegment.node_custom(
                 user_id=3202123263,
-                nickname="AAA星佑批发（Hx限定）",
+                nickname="AAA星佑批发（幻歆限定）",
                 content=Message(f"(来源)[bot]\n{text}"),                    
                 ))
         msg_list.insert(
             0,
                 MessageSegment.node_custom(
                     user_id=3485462167,
                     nickname="AAA星佑批发（幻歆限定）",
                     content=Message(f"(来源)[{nick}*hx限定][{id}]\n\n共查找到{t}条历史对话记录"),
                 ),)
     except Exception as e:
+        logger.debug(e)
         msg_list = [
             MessageSegment.node_custom(
                 user_id=3485462167,
                 nickname="AAA星佑批发（幻歆限定）",
                 content=Message("合并消息时出错！"),
             )
         ]
     return msg_list
 
+#历史消息文件获取
+def gethistorytxt(id,filename):
+    file_path=f"{log_dir}  / user / {id}"
+    if not os.path.exists(f"{file_path}"):
+        create_dir_usr(f"{file_path}")
+    filelist = os.listdir(file_path)
+    if filename+".json" in filelist:
+        return file_path / (filename+".json")
+    else:
+        return False
+
 #全局配置卡片构建
 async def get_config_global() -> List[MessageSegment]:
     config = config_in_global()
     msg_list = []
     try:
         reply = config["reply"]
         reply_at = config["reply_at"]
@@ -1495,47 +1507,44 @@
             back = back_1.json()
     except json.decoder.JSONDecodeError as e:
             back_msg = f"json解析报错！\n返回结果：{e}"
             return back_msg
     try:
         times = chat_times(id,nick)
         limit = json_get(config_in_global(),"limit")
+        msg = back['choices'][0]['message']['content']
+        ai_out(id,json_replace(msg))
         if times >= limit or times == 0:
-            msg = back['choices'][0]['message']['content']
-            ai_out(id,json_replace(text))
             back_msg = f"{msg}\n[时间线..重启.]"
         else:
-            msg = back['choices'][0]['message']['content']
-            ai_out(id,json_replace(text))
             back_msg = f"{msg}\n[{times}|{limit}]"
     except Exception as e:
         back_msg = f"api原内容{back}\n\n捕获报错:{e}\n\n未知错误，错误定位于#主要构建函数。"
+        img = await error_oops()
         if groupid:
-            img = await error_oops()
             await nonebot.get_bot().call_api("send_group_msg",group_id=groupid,message=MessageSegment.image(img))
         else:
-            img = await error_oops()
             await nonebot.get_bot().call_api("send_private_msg",user_id=id,message=MessageSegment.image(img))
     return back_msg
 
 #获取回复（被艾特）
 async def get_answer_at(matcher, event, bot):
     text = unescape(await gen_chat_text(event, bot))
     groupid = get_groupid(event)
     id = get_id(event)
     nick = await get_nick(bot,event)
     img = await get_img_urls(event)
-    user_in(id,json_replace(text))
     if  (text == "" or text == None or text == "！d" or text == "/！d") and img == []:
         if text == "！d" or text == "/！d":
             return
         else:
             msg = "诶唔，你叫我是有什么事嘛？"
             await send_msg(matcher,event,msg)
-    elif img != []:
+    user_in(id,json_replace(text))
+    if img != []:
         in_img = await image_check(img[0])
         if text == "" or text == None:
             back_msg = str(await yinying(groupid,id,"看看这个图片",nick,in_img))
         else:
             back_msg = str(await yinying(groupid,id,text,nick,in_img))
         msg = back_msg.replace("/n","\n")
         await send_msg(matcher,event,msg)
@@ -1547,19 +1556,19 @@
 #获取回复（指令触发）
 async def get_answer_ml(matcher, event ,bot ,msg):
     text = msg.extract_plain_text()
     img = await get_img_urls(event)
     groupid = get_groupid(event)
     id = get_id(event)
     nick = await get_nick(bot,event)
-    user_in(id,json_replace(text))
     if  (text == "" or text == None) and img == []:
         msg = "诶唔，你叫我是有什么事嘛？"
         await send_msg(matcher,event,msg)
-    elif img != []:
+    user_in(id,json_replace(text))
+    if img != []:
         in_img = await image_check(img[0])
         if text == "" or text == None:
             back_msg = str(await yinying(groupid,id,"看看这个图片",nick,in_img))
         else:
             back_msg = str(await yinying(groupid,id,text,nick,in_img))
         msg = back_msg.replace("/n","\n")
         await send_msg(matcher,event,msg)
```

### Comparing `nonebot-plugin-hx-yinying-1.1.9/nonebot_plugin_hx_yinying/config.py` & `nonebot-plugin-hx-yinying-1.2.0/nonebot_plugin_hx_yinying/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from typing import List, Optional, Union
 import nonebot
 from pydantic import BaseModel,AnyHttpUrl,Field
 
 
 class Config(BaseModel):
     # 插件版本号勿动！！！！
-    hx_version: Optional[str] = "1.1.9"
+    hx_version: Optional[str] = "1.2.0"
     # 秩乱v你的appid
     yinying_appid: Optional[str] = None
     # 秩乱给你的token
     yinying_token: Optional[str] = None
     # 插件数据文件存储路径，可不填。
     hx_path: Optional[str] = None
     # 图像检查api，爱来自阿里云
```

### Comparing `nonebot-plugin-hx-yinying-1.1.9/nonebot_plugin_hx_yinying/image_check.py` & `nonebot-plugin-hx-yinying-1.2.0/nonebot_plugin_hx_yinying/image_check.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 # -*- coding: utf-8 -*-
 # 引入依赖包
 # pip install alibabacloud_imageaudit20191230
-import io,json
+import io,requests,cv2
 from nonebot import get_plugin_config
 from nonebot.log import logger
 from urllib.request import urlopen
 from alibabacloud_imageaudit20191230.client import Client
 from alibabacloud_imageaudit20191230.models import ScanImageAdvanceRequestTask, ScanImageAdvanceRequest
 from alibabacloud_tea_util.models import RuntimeOptions
 from .smms import SMMS
+from PIL import Image
 from .config import Config as config_hx
 from alibabacloud_tea_openapi.models import Config
 
 
 hx_config = get_plugin_config(config_hx)
 
 config = Config(
@@ -20,44 +21,50 @@
   access_key_secret=hx_config.image_check_token,
   endpoint='imageaudit.cn-shanghai.aliyuncs.com',
   region_id='cn-shanghai'
 )
 
 async def image_upload(url:str)->str:
     smms = SMMS()
+    url = url.replace("https","http")
     img0 = urlopen(url).read()
-    img=io.BytesIO(img0)
-    file = await smms.upload(img)
+    image = Image.open(io.BytesIO(img0))
+    imgByteArr = io.BytesIO()
+    image.save(imgByteArr,format="png")
+    file = await smms.upload(imgByteArr)
     if file:
         logger.debug(f"[Hx]图片上传成功，图床链接为:{file}")
         return file
     else:
         logger.error("[Hx]图片上传失败")
         return False
 
+
+
+
 async def image_check(url:str)->str:
     img0 = await image_upload(url)
     if hx_config.image_check_appid == None or hx_config.image_check_token == None:
         logger.warning("[Hx]未配置图像检测，若因图像违规导致被封开发者id，插件开发者概不负责！！！")
-        return url
     if img0:
         logger.debug("[Hx]尝试检查图片【爱来自阿里】")
         runtime_option = RuntimeOptions()
-        img = urlopen(img0).read()
+        img = requests.get(img0).content
         task1 = ScanImageAdvanceRequestTask()
         task1.image_urlobject=io.BytesIO(img)
         scan_image_request = ScanImageAdvanceRequest(
         task=[task1],
         scene=['porn']
         )
         try:
             client = Client(config)
             response = client.scan_image_advance(scan_image_request, runtime_option)
             back = response.body.to_map()
             msg0 = back["Data"]["Results"][0]["SubResults"][0]["Rate"]
+            logger.debug(msg0)
             if msg0 <= 0.6:
                 logger.warning(f"[Hx]图片违规，请重新上传")
                 msg = False
             else:
                 msg = img0
             return msg
         except Exception as e:
```

### Comparing `nonebot-plugin-hx-yinying-1.1.9/nonebot_plugin_hx_yinying/report.py` & `nonebot-plugin-hx-yinying-1.2.0/nonebot_plugin_hx_yinying/report.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-hx-yinying-1.1.9/nonebot_plugin_hx_yinying/smms.py` & `nonebot-plugin-hx-yinying-1.2.0/nonebot_plugin_hx_yinying/smms.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-hx-yinying-1.1.9/nonebot_plugin_hx_yinying.egg-info/PKG-INFO` & `nonebot-plugin-hx-yinying-1.2.0/nonebot_plugin_hx_yinying.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-hx-yinying
-Version: 1.1.9
+Version: 1.2.0
 Summary: chat with yinying
 Home-page: https://github.com/huanxin996/nonebot_plugin_hx-yinying
 Author: Huan Xin
 Author-email: mc.xiaolang@foxmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-hx-yinying Version: 1.1.9 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-hx-yinying Version: 1.2.0 Summary:
 chat with yinying Home-page: https://github.com/huanxin996/nonebot_plugin_hx-
 yinying Author: Huan Xin Author-email: mc.xiaolang@foxmail.com Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Description-Content-
 Type: text/markdown License-File: LICENSE [![All Contributors](https://
 img.shields.io/badge/all_contributors-2-orange.svg?style=flat-square)]
 (#contributors-) * @Author : huanxin996 * @Date : 2024-4-17 * @LastEditors :
```

### Comparing `nonebot-plugin-hx-yinying-1.1.9/setup.py` & `nonebot-plugin-hx-yinying-1.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="nonebot-plugin-hx-yinying",
-    version="1.1.9",
+    version="1.2.0",
     author="Huan Xin",
     author_email="mc.xiaolang@foxmail.com",
     description="chat with yinying",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/huanxin996/nonebot_plugin_hx-yinying",
     packages=setuptools.find_packages(),
```

