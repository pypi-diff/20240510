# Comparing `tmp/Fr1997v011-1.4.5.tar.gz` & `tmp/Fr1997v011-1.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Fr1997v011-1.4.5.tar", last modified: Tue Apr 30 03:06:58 2024, max compression
+gzip compressed data, was "Fr1997v011-1.4.7.tar", last modified: Thu May  9 11:07:09 2024, max compression
```

## Comparing `Fr1997v011-1.4.5.tar` & `Fr1997v011-1.4.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-04-30 03:06:58.848653 Fr1997v011-1.4.5/
-drwxrwxrwx   0        0        0        0 2024-04-30 03:06:58.840137 Fr1997v011-1.4.5/Fr1997v011.egg-info/
--rw-rw-rw-   0        0        0      182 2024-04-30 03:06:58.000000 Fr1997v011-1.4.5/Fr1997v011.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      323 2024-04-30 03:06:58.000000 Fr1997v011-1.4.5/Fr1997v011.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-30 03:06:58.000000 Fr1997v011-1.4.5/Fr1997v011.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-04-30 03:06:58.000000 Fr1997v011-1.4.5/Fr1997v011.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       12 2024-04-30 03:06:58.000000 Fr1997v011-1.4.5/Fr1997v011.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1091 2023-10-08 06:35:50.000000 Fr1997v011-1.4.5/LICENSE
--rw-rw-rw-   0        0        0      182 2024-04-30 03:06:58.847664 Fr1997v011-1.4.5/PKG-INFO
--rw-rw-rw-   0        0        0      773 2024-04-29 18:50:20.000000 Fr1997v011-1.4.5/README.md
-drwxrwxrwx   0        0        0        0 2024-04-30 03:06:58.841137 Fr1997v011-1.4.5/fr1997_mode/
--rw-rw-rw-   0        0        0       56 2023-10-11 07:25:55.000000 Fr1997v011-1.4.5/fr1997_mode/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-30 03:06:58.844648 Fr1997v011-1.4.5/fr1997_mode/mode_func/
--rw-rw-rw-   0        0        0       29 2024-04-25 01:03:20.000000 Fr1997v011-1.4.5/fr1997_mode/mode_func/__init__.py
--rw-rw-rw-   0        0        0   175297 2024-04-30 03:06:53.000000 Fr1997v011-1.4.5/fr1997_mode/mode_func/all_func.py
-drwxrwxrwx   0        0        0        0 2024-04-30 03:06:58.845652 Fr1997v011-1.4.5/fr1997_mode/mode_static/
--rw-rw-rw-   0        0        0        0 2023-10-13 07:18:36.000000 Fr1997v011-1.4.5/fr1997_mode/mode_static/__init__.py
--rw-rw-rw-   0        0        0       42 2024-04-30 03:06:58.848653 Fr1997v011-1.4.5/setup.cfg
--rw-rw-rw-   0        0        0      322 2024-04-30 03:06:53.000000 Fr1997v011-1.4.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-09 11:07:09.201178 Fr1997v011-1.4.7/
+drwxrwxrwx   0        0        0        0 2024-05-09 11:07:09.194603 Fr1997v011-1.4.7/Fr1997v011.egg-info/
+-rw-rw-rw-   0        0        0      182 2024-05-09 11:07:09.000000 Fr1997v011-1.4.7/Fr1997v011.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      323 2024-05-09 11:07:09.000000 Fr1997v011-1.4.7/Fr1997v011.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-09 11:07:09.000000 Fr1997v011-1.4.7/Fr1997v011.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-05-09 11:07:09.000000 Fr1997v011-1.4.7/Fr1997v011.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       12 2024-05-09 11:07:09.000000 Fr1997v011-1.4.7/Fr1997v011.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1091 2023-10-08 06:35:50.000000 Fr1997v011-1.4.7/LICENSE
+-rw-rw-rw-   0        0        0      182 2024-05-09 11:07:09.200179 Fr1997v011-1.4.7/PKG-INFO
+-rw-rw-rw-   0        0        0      773 2024-05-09 11:07:08.000000 Fr1997v011-1.4.7/README.md
+drwxrwxrwx   0        0        0        0 2024-05-09 11:07:09.195592 Fr1997v011-1.4.7/fr1997_mode/
+-rw-rw-rw-   0        0        0       56 2023-10-11 07:25:55.000000 Fr1997v011-1.4.7/fr1997_mode/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-09 11:07:09.196591 Fr1997v011-1.4.7/fr1997_mode/mode_func/
+-rw-rw-rw-   0        0        0       29 2024-04-25 01:03:20.000000 Fr1997v011-1.4.7/fr1997_mode/mode_func/__init__.py
+-rw-rw-rw-   0        0        0   177160 2024-05-09 11:07:04.000000 Fr1997v011-1.4.7/fr1997_mode/mode_func/all_func.py
+drwxrwxrwx   0        0        0        0 2024-05-09 11:07:09.198094 Fr1997v011-1.4.7/fr1997_mode/mode_static/
+-rw-rw-rw-   0        0        0        0 2023-10-13 07:18:36.000000 Fr1997v011-1.4.7/fr1997_mode/mode_static/__init__.py
+-rw-rw-rw-   0        0        0       42 2024-05-09 11:07:09.201178 Fr1997v011-1.4.7/setup.cfg
+-rw-rw-rw-   0        0        0      322 2024-05-09 11:07:04.000000 Fr1997v011-1.4.7/setup.py
```

### Comparing `Fr1997v011-1.4.5/LICENSE` & `Fr1997v011-1.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `Fr1997v011-1.4.5/README.md` & `Fr1997v011-1.4.7/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 ```sh
 python setup.py sdist
 ```
 
 ### （本地）安装包
 
 ```sh
-pip install dist/Fr1997v011-1.4.4.tar.gz
+pip install dist/Fr1997v011-1.4.7.tar.gz
 ```
 
 ### 下载包
 
 ```sh
 pip install Fr1997v011
 ```
```

### Comparing `Fr1997v011-1.4.5/fr1997_mode/mode_func/all_func.py` & `Fr1997v011-1.4.7/fr1997_mode/mode_func/all_func.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,32 +25,33 @@
 
 # 腾讯云cos  pip install -U cos-python-sdk-v5
 from qcloud_cos import CosConfig
 from qcloud_cos import CosS3Client
 from django.http import JsonResponse
 
 """
+    配置文件
+        所有配置在这个地方读取 
+        使用内存缓存机制 memcache
+        没有读取到内存中的配置，这个包相当于不能用
+    pip3 cache purge
+    pip3 install -i https://pypi.tuna.tsinghua.edu.cn/simple Fr1997v011==1.4.5
+"""
+
+"""
+    pip3 install --upgrade Fr1997v011
     pip3 install redis
     pip3 install pymysql
     pip3 install elasticsearch
     pip3 install python-memcached
     pip3 install PyExecJS
     pip3 install -U cos-python-sdk-v5
     pip3 install pypinyin
 """
 
-"""
-    配置文件
-        所有配置在这个地方读取 
-        使用内存缓存机制 memcache
-        没有读取到内存中的配置，这个包相当于不能用
-    pip3 cache purge
-    pip3 install -i https://pypi.tuna.tsinghua.edu.cn/simple Fr1997v011==1.3.6
-"""
-
 
 # 存储内存数据
 def cache_set(key, data, save_time=None):
     mc = memcache.Client(['127.0.0.1:11211'], debug=True)
     if save_time:
         mc.set(key=key, val=data, time=save_time)
     else:
@@ -2173,14 +2174,102 @@
                 result = ""
         except:
             print("err ttwid_cookie获取失败")
         if result:
             return result
 
 
+# 小红书
+class XhsJike:
+
+    def xhs_web_video_main_data(self, data_json, note_id):
+        def ret_json(code=200, msg=None, data=None):
+            return {'code': code, 'msg': msg, 'data': data}
+
+        try:
+            note_info = data_json['note']['noteDetailMap'][note_id]['note']
+
+            # 关于视频链接
+            find_dld_video_url = 0
+            dld_video_url = None
+            stream = note_info['video']['media']['stream']
+            for m in stream:
+                if stream[m] and find_dld_video_url == 0:
+                    try:
+                        dld_video_url = stream[m][0]['backupUrls'][0]
+                    except:
+                        pass
+
+            if not dld_video_url:
+                return ret_json(200, '未找到url')
+
+            return ret_json(200, 'ok', {
+                'create_date': int(note_info['time'] / 1000),
+                'title': mode_text.word_change(note_info['title']),
+                'desc': mode_text.word_change(note_info['desc']),
+                'location': note_info['ipLocation'],
+                'duration': note_info['video']['capa']['duration'],
+                'dld_video_url': dld_video_url,
+
+                'nickname': mode_text.word_change(note_info['user']['nickname']),
+                'user_id': note_info['user']['userId'],
+                'avatar': note_info['user']['avatar'],
+            })
+        except Exception as e:
+            return ret_json(200, e)
+
+    def xhs_video_id_pc(self, url):
+        note_id = None
+        if '://www.xiaohongshu.com/discovery' in url:
+            note_id = url.split('://www.xiaohongshu.com/discovery/item/')[-1].split('?')[0]
+
+        if '://www.xiaohongshu.com/explore/' in url:
+            note_id = url.split('://www.xiaohongshu.com/explore/')[-1].split('?')[0]
+        return note_id
+
+    def xhs_app_url_302(self, url):
+        # app标准格式是 ://xhslink.com/s4dqRB
+        pattern = r'://xhslink\.com/([A-Za-z0-9]{6})'
+        match = re.search(pattern, url)
+        if match:
+            app_url = f'http://xhslink.com/{match.group(1)}'
+            return requests.get(app_url, headers=config_dict['base_headers']).url
+        else:
+            return None
+
+    def xhs_video_main(self, req_url, proxies=None):
+        def ret_json(code=200, msg=None, data=None):
+            return {'code': code, 'msg': msg, 'data': data}
+
+        if 'xhslink' in req_url:
+            req_url = self.xhs_app_url_302(req_url)
+            if req_url is None:
+                return ret_json(500, '未找到该视频 XHS009')
+
+        note_id = self.xhs_video_id_pc(req_url)
+        if note_id is None:
+            return ret_json(500, '未找到该视频 XHS008')
+        xhs_url = f'https://www.xiaohongshu.com/explore/{note_id}'
+        if proxies:
+            response = requests.get(xhs_url, headers=config_dict['base_headers'], proxies=proxies)
+        else:
+            response = requests.get(xhs_url, headers=config_dict['base_headers'])
+
+        true = True
+        false = False
+        null = None
+        undefined = "undefined"
+        text = response.text
+        text = text.split('window.__INITIAL_STATE__=')[-1]
+        text = text.split('</script>')[0]
+        text_json = json.loads(json.dumps(eval(text)))
+        ret_data = self.xhs_web_video_main_data(text_json, note_id)
+        return ret_data
+
+
 # django
 class DjangoJike:
     # 配置
     @staticmethod
     def django_config():
         sc = 'status_code'  # 返回码
         msg = 'message'  # 返回消息
@@ -2653,57 +2742,14 @@
                 hits_list = response.get('hits')['hits']
                 print(f'总个数:{value} 取出:{len(hits_list)}')
                 if ret_num == 0:
                     return hits_list
                 else:
                     return [hits_list, value]
 
-    # ES 查询
-    def es_search_new_20231215_old(self, table, query, _source, size=1, sort_info=None, is_ret_num=1, ret_num=0,
-                                   **kwargs):
-        body = {
-            "query": query,
-            "track_total_hits": True if is_ret_num == 1 else False,
-            "size": size,
-            "_source": _source,
-        }
-
-        # 排序
-        if sort_info and sort_info != 0:
-            body['sort'] = sort_info
-        else:
-            body['sort'] = {
-                "_script": {
-                    "script": "Math.random()",
-                    "type": "number"
-                }
-            }
-
-        es_cfg = 'es_jike_out'
-        es_ip = config_dict['es'][es_cfg]['ip']
-        es_user = config_dict['es'][es_cfg]['user']
-        es_pwb = config_dict['es'][es_cfg]['pwd']
-        es_port = config_dict['es'][es_cfg]['port']
-        es = Elasticsearch([f'{es_ip}:{es_port}'], http_auth=(es_user, es_pwb))
-        response = es.search(
-            index=table,
-            body=body
-        )
-        _shards = response.get('_shards')
-        if _shards:
-            successful = _shards.get('successful')
-            if successful > 0:
-                value = response.get('hits')['total']['value']
-                hits_list = response.get('hits')['hits']
-                print(f'总个数:{value} 取出:{len(hits_list)}')
-                if ret_num == 0:
-                    return hits_list
-                else:
-                    return [hits_list, value]
-
     # ES 查询 单条
     def es_search_one(self, table, _id, is_print=1):
         body = {
             "track_total_hits": True,
             "query": {
                 "match": {"_id": _id}
             }
@@ -4409,16 +4455,15 @@
 mode_feishu = Feishu()  # 飞书app api
 mode_time = TimeJike()  # 时间处理
 mode_text = TextJike()  # 文本处理
 mode_data = DataJike()  # 数据处理
 mode_spider = SpiderJike()  # 数据请求
 mode_django = DjangoJike()  # django配置
 mode_douyin = DouyinJike()  # douyin配置
+mode_xhs = XhsJike()  # douyin配置
 mode_pros = ModeStatic()  # 其它函数
 mode_cos = Cos()  # cos
 mode_fr_cos = Cos(server_select='personal')  # cos 高阳
 mode_myself = MyGy()
 
 mode_pro = ModeFunc()  # main
 
-# data_data = FastGptAuto(run_path=2).app_log('12419','662f0e6d9cc568621d02d0fb')
-# print(data_data)
```

