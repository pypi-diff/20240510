# Comparing `tmp/pyqqq_cli-0.2.9.tar.gz` & `tmp/pyqqq_cli-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyqqq_cli-0.2.9.tar", max compression
+gzip compressed data, was "pyqqq_cli-0.3.0.tar", max compression
```

## Comparing `pyqqq_cli-0.2.9.tar` & `pyqqq_cli-0.3.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1064 2024-04-22 08:23:09.109923 pyqqq_cli-0.2.9/README.md
--rw-r--r--   0        0        0      655 2024-05-02 09:48:21.706887 pyqqq_cli-0.2.9/pyproject.toml
--rw-r--r--   0        0        0      358 2024-05-02 09:40:11.894616 pyqqq_cli-0.2.9/qupiato/cli/config.py
--rw-r--r--   0        0        0     8773 2024-05-02 09:40:59.528982 pyqqq_cli-0.2.9/qupiato/cli/main.py
--rw-r--r--   0        0        0     7097 2024-05-02 09:45:29.468608 pyqqq_cli-0.2.9/qupiato/cli/utils.py
--rw-r--r--   0        0        0     1936 1970-01-01 00:00:00.000000 pyqqq_cli-0.2.9/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-04-22 08:23:09.109923 pyqqq_cli-0.3.0/README.md
+-rw-r--r--   0        0        0      655 2024-05-10 08:56:21.840734 pyqqq_cli-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      358 2024-05-10 08:53:22.816157 pyqqq_cli-0.3.0/qupiato/cli/config.py
+-rw-r--r--   0        0        0     8797 2024-05-10 08:24:10.048864 pyqqq_cli-0.3.0/qupiato/cli/main.py
+-rw-r--r--   0        0        0     7239 2024-05-10 08:53:22.817467 pyqqq_cli-0.3.0/qupiato/cli/utils.py
+-rw-r--r--   0        0        0     1936 1970-01-01 00:00:00.000000 pyqqq_cli-0.3.0/PKG-INFO
```

### Comparing `pyqqq_cli-0.2.9/README.md` & `pyqqq_cli-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `pyqqq_cli-0.2.9/pyproject.toml` & `pyqqq_cli-0.3.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyqqq-cli"
-version = "0.2.9"
+version = "0.3.0"
 description = "CLI tool for controlling strategies deployed on the PyQQQ platform."
 authors = ["PyQQQ team <pyqqq.cs@gmail.com>"]
 readme = "README.md"
 packages = [{include = "qupiato"}]
 license = "MIT"
 documentation = "https://qupiato-sdk-18secs-cf54ebea1b14b422537daf0462fb86d68f4582d064a4.gitlab.io"
```

### Comparing `pyqqq_cli-0.2.9/qupiato/cli/main.py` & `pyqqq_cli-0.3.0/qupiato/cli/main.py`

 * *Files 20% similar despite different names*

```diff
@@ -69,17 +69,19 @@
     }
 
     async for line in ws_api_call(req):
         if 'text' in line:
             click.echo(line['text'])
 
     if publish:
-        click.echo("Publishing strategy")
-        publish_strategy(entryfile, strategy_name)
-
+        try:
+            publish_strategy(entryfile, strategy_name, zipfile)
+            click.echo(f"Publishing {entryfile} as {strategy_name} to public repository")
+        except Exception as e:
+            click.echo(e)
 
 @main.command()
 def list():
     """ List deployed strategies """
 
     asyncio.run(list_strategies())
 
@@ -242,15 +244,15 @@
 
 @main.command()
 @click.argument('term', required=False)
 @click.option('--email', '-e', default=None, help="Specify email to search for")
 def search(term, email):
     """ Search for stock investment strategies """
     params = {
-        "query": term
+        "term": term
     }
     if email is not None:
         params['email'] = email
 
     r = search_strategies(params)
 
     if r is None or 'data' not in r or len(r['data']) == 0:
@@ -268,48 +270,47 @@
 @main.command()
 @click.argument('name')
 def pull(name):
     """ Download an strategy from the registry """
     [email, strategy_name] = name.split('/')
 
     params = {
-        'email': email,
-        'query': strategy_name
+        'term': strategy_name,
+        'email': email
     }
     r = search_strategies(params)
 
     if r is None or 'data' not in r or len(r['data']) == 0:
         click.echo("Strategy does not exists or not accessible")
         sys.exit(1)
     elif len(r['data']) > 1:
         click.echo("Strategy is ambiguous, please specify the name")
         __format_strategies(r['data'])
         sys.exit(1)
 
-    file_name = r['data'][0]['file']
+    file_name = r['data'][0]['zipfile']
     pull_strategy(strategy_name, file_name)
 
     click.echo(f"{name}'s download has completed")
 
 
 def __format_strategies(data):
+    display = []
     for e in data:
-        user_info = get_user(e['user'])
-        email = user_info['email']
-        e.update({
-            'id': f"{email}/{e['name']}",
-            'user': e['user']
+        display.append({
+            'name': f"{e['email']}/{e['strategy_name']}",
+            'user': e['uid'],
+            'star': str(e['extra_info']['star'])
         })
 
-    name_width = __calc_column_width(data, 'id', "NAME")
-    user_width = __calc_column_width(data, 'user', "USER")
-    status_width = __calc_column_width(data, 'active', "STATUS")
+    name_width = __calc_column_width(display, 'name', "NAME")
+    user_width = __calc_column_width(display, 'user', "USER")
+    star_width = __calc_column_width(display, 'star', "STAR")
 
-    click.echo(f"{'NAME':<{name_width}} {'USER':<{user_width}} {'VERSION':<{status_width}} CREATED AT")
+    click.echo(f"{'NAME':<{name_width}} {'USER':<{user_width}} {'STAR':<{star_width}}")
 
-    for e in data:
-        created_at = dtm.datetime.fromisoformat(e['created_at']).strftime('%Y-%m-%d %H:%M:%S')
-        click.echo(f"{e['id']:<{name_width}} {e['user']:<{user_width}} {e['revision']:<{status_width}} {created_at}")
+    for e in display:
+        click.echo(f"{e['name']:<{name_width}} {e['user']:<{user_width}} {e['star']:<{star_width}}")
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `pyqqq_cli-0.2.9/qupiato/cli/utils.py` & `pyqqq_cli-0.3.0/qupiato/cli/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -106,25 +106,26 @@
         return object_key
 
 def get_version():
     version = importlib.metadata.version('pyqqq-cli')
     return version
 
 def search_strategies(params=''):
-    url = f"{c.API_SERVER_URL}/deployments/search"
+    url = f"{c.API_SERVER_URL}/strategy/publish"
     headers = {
         'Authorization': f'Bearer {get_token()}'
     }
     response = requests.get(url, headers=headers, params=params)
 
     if response.status_code != 200:
         if response.status_code == 404:
             return None
         else:
-            raise Exception("Failed to search strategies")
+            code, message = response.json().values()
+            raise Exception(f"Failed to search strategies {message}")
 
     return response.json()
 
 def pull_strategy(name, filename):
     url = f"{c.API_SERVER_URL}/deployments/download"
     headers = {
         'Authorization': f'Bearer {get_token()}'
@@ -138,15 +139,15 @@
         for chunk in response.iter_content(None):
             buffer.write(chunk)
 
         with zipfile.ZipFile(buffer) as zipf:
             zipf.extractall(name)
 
 # 전략의 공개 설정
-def publish_strategy(entryfile, strategy_name):
+def publish_strategy(entryfile, strategy_name, zipfile):
     entry_dir = os.path.dirname(os.path.normpath(entryfile))
     markdown = None
     for root, _, files in os.walk(entry_dir or '.'):
         if markdown is not None:
             break
 
         for file in files:
@@ -158,24 +159,27 @@
                 markdown = norm_path
                 break
 
     url = f"{c.API_SERVER_URL}/strategy/publish"
     headers = {
         'Authorization': f'Bearer {get_token()}'
     }
-    payload = { 'strategy': strategy_name }
+    payload = {
+        'strategy': strategy_name,
+        'zipfile': zipfile,
+    }
 
     if markdown:
         files = { 'file': (os.path.basename(markdown), open(markdown, 'rb'), 'application/octet-stream') }
         response = requests.post(url, headers=headers, files=files, data=payload)
     else:
         response = requests.post(url, headers=headers, data=payload)
 
     if response.status_code != 200 and response.status_code != 201:
-        raise Exception("Publish failed to strategies")
+        raise Exception(f"Publishing failed with status code {response.status_code}")
 
     return response.json()
 
 # 사용자 정보 조회
 def get_user(uid):
     url = f"{c.API_SERVER_URL}/user"
     headers = {
```

### Comparing `pyqqq_cli-0.2.9/PKG-INFO` & `pyqqq_cli-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyqqq-cli
-Version: 0.2.9
+Version: 0.3.0
 Summary: CLI tool for controlling strategies deployed on the PyQQQ platform.
 License: MIT
 Author: PyQQQ team
 Author-email: pyqqq.cs@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

