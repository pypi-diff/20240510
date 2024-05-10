# Comparing `tmp/yt_music-0.0.7.tar.gz` & `tmp/yt_music-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yt_music-0.0.7.tar", max compression
+gzip compressed data, was "yt_music-0.0.8.tar", max compression
```

## Comparing `yt_music-0.0.7.tar` & `yt_music-0.0.8.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    35149 2024-02-21 19:01:59.066884 yt_music-0.0.7/LICENSE
--rw-r--r--   0        0        0      506 2024-02-21 19:01:59.066884 yt_music-0.0.7/pyproject.toml
--rw-r--r--   0        0        0        0 2024-02-21 19:01:59.066884 yt_music-0.0.7/readme.txt
--rw-r--r--   0        0        0        0 2024-02-21 19:01:59.066884 yt_music-0.0.7/yt_music/__init__.py
--rw-r--r--   0        0        0      110 2024-02-21 19:01:59.066884 yt_music-0.0.7/yt_music/__main__.py
--rw-r--r--   0        0        0       19 2024-02-21 19:01:59.066884 yt_music-0.0.7/yt_music/__version__.py
--rw-r--r--   0        0        0     4377 2024-02-21 19:01:59.066884 yt_music-0.0.7/yt_music/__yt_music__.py
--rw-r--r--   0        0        0      647 1970-01-01 00:00:00.000000 yt_music-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-05-10 16:53:31.935077 yt_music-0.0.8/LICENSE
+-rw-r--r--   0        0        0      521 2024-05-10 16:53:31.935077 yt_music-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-10 16:53:31.935077 yt_music-0.0.8/readme.txt
+-rw-r--r--   0        0        0        0 2024-05-10 16:53:31.935077 yt_music-0.0.8/yt_music/__init__.py
+-rw-r--r--   0        0        0      110 2024-05-10 16:53:31.935077 yt_music-0.0.8/yt_music/__main__.py
+-rw-r--r--   0        0        0       19 2024-05-10 16:53:31.935077 yt_music-0.0.8/yt_music/__version__.py
+-rw-r--r--   0        0        0     4979 2024-05-10 16:53:31.935077 yt_music-0.0.8/yt_music/__yt_music__.py
+-rw-r--r--   0        0        0      683 1970-01-01 00:00:00.000000 yt_music-0.0.8/PKG-INFO
```

### Comparing `yt_music-0.0.7/LICENSE` & `yt_music-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `yt_music-0.0.7/yt_music/__yt_music__.py` & `yt_music-0.0.8/yt_music/__yt_music__.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import os
 import time
 import html
 import json
 
 import httpx
 import fzf
+from bs4 import BeautifulSoup as bs
 
 plt = platform.system()
 username = os.getenv('username') if plt == 'Windows' else os.getlogin()
 config_path = os.path.join(os.path.expanduser(f'~{username}'), '.config', 'yt-music', 'config.json')
 
 if os.path.exists(config_path):
     with open(config_path) as f:
@@ -33,14 +34,15 @@
     RPC = Presence(client_id)
     RPC.connect()
 
 client = httpx.Client(headers=headers, timeout=None)
 
 base_url = "https://vid.puffyan.us"
 pattern = r'<a.*?href="/watch\?v=(.*?)".*?><p.*?>(.*?)<\/p></a>'
+channel_name_pattern = r'<span id="channel-name">(.*?)</span>'
 
 MPV_EXECUTABLE = "mpv"
 
 try:
     if len(sys.argv) == 1:
         query = input("Search: ")
         if query == "":
@@ -51,24 +53,37 @@
 except KeyboardInterrupt:
     exit(0)
 
 query = query.replace(' ', '+')
 opts = []
 
 
+def get_channel(video_id):
+    resp = client.get(f"https://vid.puffyan.us/watch?v={video_id}")
+    html_content = resp.text
+    soup = bs(html_content, 'html.parser')
+    channel_names = re.findall(channel_name_pattern, html_content)
+
+    for name in channel_names:
+        print(name.strip())
+        get_channel.artist = name.strip()
+
+
 def extract_video_id(video_title):
     match = re.search(r' - ([\w-]+)$', video_title)
     
     #match = re.search(pattern, video_title)
     
     if match:
         video_id = match.group(1)
+        get_channel(video_id)
         return video_id
     else:
-        return None
+        print("no video id found")
+        exit(1)
 
 def determine_path() -> str:
     
     if plt == "Windows":
         return f"C:\\Users\\{os.getenv('username')}\\Downloads"
     
     elif (plt == "Linux"):
@@ -85,24 +100,26 @@
     
     path: str = determine_path()
     video_title = video_title.replace(' ', '_')
 
     subprocess.call(f"yt-dlp -x \"https://music.youtube.com/watch?v={video_id}\" -o \"{path}/{video_title}\"", shell=True)
 
 
+
 def play_loop(video_id, video_title):
    
     if use_rpc == "true":
         RPC.update(
             large_image = f"http://img.youtube.com/vi/{video_id}/0.jpg",
             large_text = "haha checkmate spotify plebs",
             small_image = "youtube_music_icon_svg",
-            small_text = "yt-music",
+            small_text = f"yt-music",
             start = start,
             details = f"{video_title} - loop",
+            state = f"by {get_channel.artist}",
             buttons = [{"label": "Play on YouTube Music", "url": f"https://music.youtube.com/watch?v={video_id}"}],
         )
 
     args = [
         MPV_EXECUTABLE,
         f"https://music.youtube.com/watch?v={video_id}",
         f"--force-media-title={video_title}",
@@ -118,17 +135,18 @@
 def play(video_id, video_title):
    
     if use_rpc == "true":
         RPC.update(
             large_image = f"http://img.youtube.com/vi/{video_id}/0.jpg",
             large_text = "haha checkmate spotify plebs",
             small_image = "youtube_music_icon_svg",
-            small_text = "yt-music",
+            small_text = f"yt-music",
             start = start,
-            details = video_title,
+            details = f"{video_title}",
+            state = f"by {get_channel.artist}",
             buttons = [{"label": "Play on YouTube Music", "url": f"https://music.youtube.com/watch?v={video_id}"}],
         )
 
     args = [
         MPV_EXECUTABLE,
         f"https://music.youtube.com/watch?v={video_id}",
         f"--force-media-title={video_title}",
```

### Comparing `yt_music-0.0.7/PKG-INFO` & `yt_music-0.0.8/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: yt-music
-Version: 0.0.7
+Version: 0.0.8
 Summary: A command line YouTube Music client.
 License: GPLv3
 Author: DemonKingSwarn
 Author-email: rockingswarn@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: bs4 (>=0.0.2,<0.0.3)
 Requires-Dist: httpx (==0.23.0)
 Requires-Dist: krfzf-py (>=0.0.4,<0.0.5)
 Requires-Dist: pypresence (==4.3.0)
 Requires-Dist: yt-dlp (>=2023.12.30,<2024.0.0)
 Description-Content-Type: text/plain
```

