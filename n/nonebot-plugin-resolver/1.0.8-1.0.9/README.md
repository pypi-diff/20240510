# Comparing `tmp/nonebot_plugin_resolver-1.0.8.tar.gz` & `tmp/nonebot_plugin_resolver-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_resolver-1.0.8.tar", max compression
+gzip compressed data, was "nonebot_plugin_resolver-1.0.9.tar", max compression
```

## Comparing `nonebot_plugin_resolver-1.0.8.tar` & `nonebot_plugin_resolver-1.0.9.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    13566 2023-02-16 15:40:41.683633 nonebot_plugin_resolver-1.0.8/nonebot-plugin-resolver/__init__.py
--rw-r--r--   0        0        0     4279 2023-02-16 08:27:09.540780 nonebot_plugin_resolver-1.0.8/nonebot-plugin-resolver/acfun_utils.py
--rw-r--r--   0        0        0     2992 2023-02-16 08:49:32.884612 nonebot_plugin_resolver-1.0.8/nonebot-plugin-resolver/bili23_utils.py
--rw-r--r--   0        0        0     2960 2023-02-16 08:41:49.053046 nonebot_plugin_resolver-1.0.8/nonebot-plugin-resolver/common_utils.py
--rw-r--r--   0        0        0      304 2023-02-16 08:27:09.514781 nonebot_plugin_resolver-1.0.8/nonebot-plugin-resolver/tiktok_utills.py
--rw-r--r--   0        0        0      204 2023-02-16 08:41:49.057046 nonebot_plugin_resolver-1.0.8/nonebot-plugin-resolver/twitter_utils.py
--rw-r--r--   0        0        0        0 2023-02-16 08:12:05.385391 nonebot_plugin_resolver-1.0.8/nonebot-plugin-resolver/xhs_utils.py
--rw-r--r--   0        0        0      723 2023-02-16 16:02:44.002929 nonebot_plugin_resolver-1.0.8/pyproject.toml
--rw-r--r--   0        0        0     1646 2023-02-16 16:07:56.464735 nonebot_plugin_resolver-1.0.8/README.md
--rw-r--r--   0        0        0     2581 1970-01-01 00:00:00.000000 nonebot_plugin_resolver-1.0.8/setup.py
--rw-r--r--   0        0        0     2560 1970-01-01 00:00:00.000000 nonebot_plugin_resolver-1.0.8/PKG-INFO
+-rw-r--r--   0        0        0    13557 2023-02-16 16:48:33.888227 nonebot_plugin_resolver-1.0.9/nonebot-plugin-resolver/__init__.py
+-rw-r--r--   0        0        0     4279 2023-02-16 08:27:09.540780 nonebot_plugin_resolver-1.0.9/nonebot-plugin-resolver/acfun_utils.py
+-rw-r--r--   0        0        0     2992 2023-02-16 08:49:32.884612 nonebot_plugin_resolver-1.0.9/nonebot-plugin-resolver/bili23_utils.py
+-rw-r--r--   0        0        0     2960 2023-02-16 08:41:49.053046 nonebot_plugin_resolver-1.0.9/nonebot-plugin-resolver/common_utils.py
+-rw-r--r--   0        0        0      304 2023-02-16 08:27:09.514781 nonebot_plugin_resolver-1.0.9/nonebot-plugin-resolver/tiktok_utills.py
+-rw-r--r--   0        0        0      204 2023-02-16 08:41:49.057046 nonebot_plugin_resolver-1.0.9/nonebot-plugin-resolver/twitter_utils.py
+-rw-r--r--   0        0        0        0 2023-02-16 08:12:05.385391 nonebot_plugin_resolver-1.0.9/nonebot-plugin-resolver/xhs_utils.py
+-rw-r--r--   0        0        0      723 2023-02-16 16:48:45.906391 nonebot_plugin_resolver-1.0.9/pyproject.toml
+-rw-r--r--   0        0        0     1646 2023-02-16 16:07:56.464735 nonebot_plugin_resolver-1.0.9/README.md
+-rw-r--r--   0        0        0     2581 1970-01-01 00:00:00.000000 nonebot_plugin_resolver-1.0.9/setup.py
+-rw-r--r--   0        0        0     2560 1970-01-01 00:00:00.000000 nonebot_plugin_resolver-1.0.9/PKG-INFO
```

### Comparing `nonebot_plugin_resolver-1.0.8/nonebot-plugin-resolver/__init__.py` & `nonebot_plugin_resolver-1.0.9/nonebot-plugin-resolver/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from .bili23_utils import getDownloadUrl, downloadBFile, mergeFileToMp4, get_dynamic
 from .tiktok_utills import get_id_video
 from .acfun_utils import parse_url, download_m3u8_videos, parse_m3u8, merge_ac_file_to_mp4
 from .twitter_utils import TweepyWithProxy
 
 
 # 全局配置
-global_config = get_driver().config.dict()
+global_config = get_driver().config
 resolver_proxy = getattr(global_config, "resolver_proxy", "http://127.0.0.1:7890")
 
 # twitter 代理地址
 proxies = {
     'http': resolver_proxy,
     'https': resolver_proxy
 }
@@ -30,15 +30,14 @@
     "https://": resolver_proxy,
 }
 
 # Twitter token
 client = TweepyWithProxy(
     proxies,
     getattr(global_config, "bearer_token", ""))
-
 bili23 = on_regex(
     r"(.*)(bilibili.com|b23.tv)", priority=1
 )
 @bili23.handle()
 async def bilibili(event: Event) -> None:
     """
         哔哩哔哩解析
```

### Comparing `nonebot_plugin_resolver-1.0.8/nonebot-plugin-resolver/acfun_utils.py` & `nonebot_plugin_resolver-1.0.9/nonebot-plugin-resolver/acfun_utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_resolver-1.0.8/nonebot-plugin-resolver/bili23_utils.py` & `nonebot_plugin_resolver-1.0.9/nonebot-plugin-resolver/bili23_utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_resolver-1.0.8/nonebot-plugin-resolver/common_utils.py` & `nonebot_plugin_resolver-1.0.9/nonebot-plugin-resolver/common_utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_resolver-1.0.8/pyproject.toml` & `nonebot_plugin_resolver-1.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-resolver"
-version = "1.0.8"
+version = "1.0.9"
 description = "NoneBot2的解析视频、图片链接/小程序插件，tiktok、bilibili、twitter等实时发送"
 authors = ["zhiyu1998 <renzhiyu0416@qq.com>"]
 readme = "README.md"
 packages = [{include = "nonebot-plugin-resolver"}]
 repository = "https://github.com/zhiyu1998/nonebot_plugin_resolver"
 keywords = ["nonebot", "nonebot2", "resolver"]
```

### Comparing `nonebot_plugin_resolver-1.0.8/README.md` & `nonebot_plugin_resolver-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_resolver-1.0.8/setup.py` & `nonebot_plugin_resolver-1.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
  'lxml>=4.9,<5.0',
  'nonebot-adapter-onebot>=2.0.0-beta.1,<3.0.0',
  'nonebot2>=2.0.0-beta.5,<3.0.0',
  'tweepy>=4.12,<5.0']
 
 setup_kwargs = {
     'name': 'nonebot-plugin-resolver',
-    'version': '1.0.8',
+    'version': '1.0.9',
     'description': 'NoneBot2的解析视频、图片链接/小程序插件，tiktok、bilibili、twitter等实时发送',
     'long_description': '<div align="center">\n  <a href="https://v2.nonebot.dev/store"><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/nbp_logo.png" width="180" height="180" alt="NoneBotPluginLogo"></a>\n  <br>\n  <p><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/NoneBotPlugin.svg" width="240" alt="NoneBotPluginText"></p>\n</div>\n\n<div align="center">\n\n# nonebot-plugin-resolver\n\n_✨ NoneBot2 解析视频、图片链接/小程序插件 ✨_\n\n\n<a href="./LICENSE">\n    <img src="https://img.shields.io/github/license/owner/nonebot-plugin-resolver.svg" alt="license">\n</a>\n<a href="https://pypi.org/project/nonebot-plugin-resolver">\n    <img src="https://img.shields.io/pypi/v/nonebot-plugin-resolver.svg" alt="pypi">\n</a>\n<img src="https://img.shields.io/badge/python-3.9+-blue.svg" alt="python">\n\n</div>\n\n## 📖 介绍\n\n适用于NoneBot2的解析视频、图片链接/小程序插件，tiktok、bilibili、twitter等实时发送！\n## 💿 安装\n\n1. 使用 nb-cli 安装，不需要手动添加入口，更新使用 pip\n\n```\nnb plugin install nonebot_plugin_resolver\n```\n\n2. 使用 pip 安装和更新，初次安装需要手动添加入口\n\n```\npip install --upgrade nonebot_plugin_resolver\n```\n\n## ⚙️ 配置\n\n在 nonebot2 项目的`.env`文件中添加下表中的必填配置\n\n```\n# twitter的token和本地代理\nbearer_token = ""\nresolver_proxy = "http://127.0.0.1:7890"\n```\n\n## 🎉 使用 & 效果图\n![help](./img/example.png)\n![help](./img/example2.png)\n![help](./img/example3.png)\n![help](./img/example4.png)\n![help](./img/example5.png)\n\n',
     'author': 'zhiyu1998',
     'author_email': 'renzhiyu0416@qq.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/zhiyu1998/nonebot_plugin_resolver',
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*- from setuptools import setup packages = \ ['nonebot-
 plugin-resolver'] package_data = \ {'': ['*']} install_requires = \
 ['aiohttp>=3.7,<4.0', 'beautifulsoup4>=4.11,<5.0', 'httpx>=0.23,<0.24',
 'lxml>=4.9,<5.0', 'nonebot-adapter-onebot>=2.0.0-beta.1,<3.0.0',
 'nonebot2>=2.0.0-beta.5,<3.0.0', 'tweepy>=4.12,<5.0'] setup_kwargs = { 'name':
-'nonebot-plugin-resolver', 'version': '1.0.8', 'description':
+'nonebot-plugin-resolver', 'version': '1.0.9', 'description':
 'NoneBot2çè§£æè§é¢ãå¾çé¾æ¥/
 å°ç¨åºæä»¶ï¼tiktokãbilibiliãtwitterç­å®æ¶åé',
 'long_description': '
                            \n _[_N_o_n_e_B_o_t_P_l_u_g_i_n_L_o_g_o_]\n
                                       \n
                               [NoneBotPluginText]
                                       \n
```

### Comparing `nonebot_plugin_resolver-1.0.8/PKG-INFO` & `nonebot_plugin_resolver-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-resolver
-Version: 1.0.8
+Version: 1.0.9
 Summary: NoneBot2的解析视频、图片链接/小程序插件，tiktok、bilibili、twitter等实时发送
 Home-page: https://github.com/zhiyu1998/nonebot_plugin_resolver
 Keywords: nonebot,nonebot2,resolver
 Author: zhiyu1998
 Author-email: renzhiyu0416@qq.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-resolver Version: 1.0.8 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-resolver Version: 1.0.9 Summary:
 NoneBot2çè§£æè§é¢ãå¾çé¾æ¥/
 å°ç¨åºæä»¶ï¼tiktokãbilibiliãtwitterç­å®æ¶åé Home-page: https:/
 /github.com/zhiyu1998/nonebot_plugin_resolver Keywords:
 nonebot,nonebot2,resolver Author: zhiyu1998 Author-email: renzhiyu0416@qq.com
 Requires-Python: >=3.9,<4.0 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
```

