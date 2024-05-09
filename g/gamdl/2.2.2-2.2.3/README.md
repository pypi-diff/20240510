# Comparing `tmp/gamdl-2.2.2.tar.gz` & `tmp/gamdl-2.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gamdl-2.2.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "gamdl-2.2.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `gamdl-2.2.2.tar` & `gamdl-2.2.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0       17 2024-04-25 00:31:31.000473 gamdl-2.2.2/.github/FUNDING.yml
--rw-r--r--   0        0        0     1137 2024-04-25 00:31:31.000473 gamdl-2.2.2/.github/workflows/main.yml
--rw-r--r--   0        0        0       79 2024-04-25 00:31:31.000473 gamdl-2.2.2/.gitignore
--rw-r--r--   0        0        0    12217 2024-04-25 00:31:31.000473 gamdl-2.2.2/README.md
--rw-r--r--   0        0        0       22 2024-04-25 00:31:31.000473 gamdl-2.2.2/gamdl/__init__.py
--rw-r--r--   0        0        0       30 2024-04-25 00:31:31.000473 gamdl-2.2.2/gamdl/__main__.py
--rw-r--r--   0        0        0     8853 2024-04-25 00:31:31.000473 gamdl-2.2.2/gamdl/apple_music_api.py
--rw-r--r--   0        0        0    26865 2024-04-25 00:31:31.000473 gamdl-2.2.2/gamdl/cli.py
--rw-r--r--   0        0        0     5570 2024-04-25 00:31:31.000473 gamdl-2.2.2/gamdl/constants.py
--rw-r--r--   0        0        0    16173 2024-04-25 00:31:31.000473 gamdl-2.2.2/gamdl/downloader.py
--rw-r--r--   0        0        0    10263 2024-04-25 00:31:31.000473 gamdl-2.2.2/gamdl/downloader_music_video.py
--rw-r--r--   0        0        0     2202 2024-04-25 00:31:31.000473 gamdl-2.2.2/gamdl/downloader_post.py
--rw-r--r--   0        0        0    14146 2024-04-25 00:31:31.000473 gamdl-2.2.2/gamdl/downloader_song.py
--rw-r--r--   0        0        0     3882 2024-04-25 00:31:31.000473 gamdl-2.2.2/gamdl/downloader_song_legacy.py
--rw-r--r--   0        0        0      797 2024-04-25 00:31:31.000473 gamdl-2.2.2/gamdl/enums.py
--rw-r--r--   0        0        0     4015 2024-04-25 00:31:31.004473 gamdl-2.2.2/gamdl/hardcoded_wvd.py
--rw-r--r--   0        0        0     2418 2024-04-25 00:31:31.004473 gamdl-2.2.2/gamdl/itunes_api.py
--rw-r--r--   0        0        0      369 2024-04-25 00:31:31.004473 gamdl-2.2.2/gamdl/models.py
--rw-r--r--   0        0        0      593 2024-04-25 00:31:31.004473 gamdl-2.2.2/pyproject.toml
--rw-r--r--   0        0        0       56 2024-04-25 00:31:31.004473 gamdl-2.2.2/requirements.txt
--rw-r--r--   0        0        0    12725 1970-01-01 00:00:00.000000 gamdl-2.2.2/PKG-INFO
+-rw-r--r--   0        0        0       17 2024-05-09 23:19:48.259539 gamdl-2.2.3/.github/FUNDING.yml
+-rw-r--r--   0        0        0     1137 2024-05-09 23:19:48.259539 gamdl-2.2.3/.github/workflows/main.yml
+-rw-r--r--   0        0        0       79 2024-05-09 23:19:48.259539 gamdl-2.2.3/.gitignore
+-rw-r--r--   0        0        0    12216 2024-05-09 23:19:48.259539 gamdl-2.2.3/README.md
+-rw-r--r--   0        0        0       22 2024-05-09 23:19:48.259539 gamdl-2.2.3/gamdl/__init__.py
+-rw-r--r--   0        0        0       30 2024-05-09 23:19:48.259539 gamdl-2.2.3/gamdl/__main__.py
+-rw-r--r--   0        0        0     8853 2024-05-09 23:19:48.259539 gamdl-2.2.3/gamdl/apple_music_api.py
+-rw-r--r--   0        0        0    26865 2024-05-09 23:19:48.259539 gamdl-2.2.3/gamdl/cli.py
+-rw-r--r--   0        0        0     5570 2024-05-09 23:19:48.259539 gamdl-2.2.3/gamdl/constants.py
+-rw-r--r--   0        0        0    16263 2024-05-09 23:19:48.259539 gamdl-2.2.3/gamdl/downloader.py
+-rw-r--r--   0        0        0    10263 2024-05-09 23:19:48.259539 gamdl-2.2.3/gamdl/downloader_music_video.py
+-rw-r--r--   0        0        0     2202 2024-05-09 23:19:48.259539 gamdl-2.2.3/gamdl/downloader_post.py
+-rw-r--r--   0        0        0    14146 2024-05-09 23:19:48.259539 gamdl-2.2.3/gamdl/downloader_song.py
+-rw-r--r--   0        0        0     4016 2024-05-09 23:19:48.259539 gamdl-2.2.3/gamdl/downloader_song_legacy.py
+-rw-r--r--   0        0        0      797 2024-05-09 23:19:48.259539 gamdl-2.2.3/gamdl/enums.py
+-rw-r--r--   0        0        0     4015 2024-05-09 23:19:48.259539 gamdl-2.2.3/gamdl/hardcoded_wvd.py
+-rw-r--r--   0        0        0     2418 2024-05-09 23:19:48.259539 gamdl-2.2.3/gamdl/itunes_api.py
+-rw-r--r--   0        0        0      369 2024-05-09 23:19:48.259539 gamdl-2.2.3/gamdl/models.py
+-rw-r--r--   0        0        0      593 2024-05-09 23:19:48.259539 gamdl-2.2.3/pyproject.toml
+-rw-r--r--   0        0        0       56 2024-05-09 23:19:48.259539 gamdl-2.2.3/requirements.txt
+-rw-r--r--   0        0        0    12724 1970-01-01 00:00:00.000000 gamdl-2.2.3/PKG-INFO
```

### Comparing `gamdl-2.2.2/.github/workflows/main.yml` & `gamdl-2.2.3/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `gamdl-2.2.2/README.md` & `gamdl-2.2.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -187,8 +187,7 @@
     * Native format for Apple Music synced lyrics.
     * Highly unsupported by media players.
   
 ### Cover formats
 The following cover formats are available:
 * `jpg`
 * `png`
-
```

### Comparing `gamdl-2.2.2/gamdl/apple_music_api.py` & `gamdl-2.2.3/gamdl/apple_music_api.py`

 * *Files identical despite different names*

### Comparing `gamdl-2.2.2/gamdl/cli.py` & `gamdl-2.2.3/gamdl/cli.py`

 * *Files identical despite different names*

### Comparing `gamdl-2.2.2/gamdl/constants.py` & `gamdl-2.2.3/gamdl/constants.py`

 * *Files identical despite different names*

### Comparing `gamdl-2.2.2/gamdl/downloader.py` & `gamdl-2.2.3/gamdl/downloader.py`

 * *Files 0% similar despite different names*

```diff
@@ -248,29 +248,31 @@
         return f"{minutes:02d}:{seconds:02d}"
 
     def sanitize_date(self, date: str):
         datetime_obj = ciso8601.parse_datetime(date)
         return datetime_obj.strftime(self.template_date)
 
     def get_decryption_key(self, pssh: str, track_id: str) -> str:
-        pssh_obj = PSSH(pssh.split(",")[-1])
-        cdm_session = self.cdm.open()
-        challenge = base64.b64encode(
-            self.cdm.get_license_challenge(cdm_session, pssh_obj)
-        ).decode()
-        license = self.apple_music_api.get_widevine_license(
-            track_id,
-            pssh,
-            challenge,
-        )
-        self.cdm.parse_license(cdm_session, license)
-        decryption_key = next(
-            i for i in self.cdm.get_keys(cdm_session) if i.type == "CONTENT"
-        ).key.hex()
-        self.cdm.close(cdm_session)
+        try:
+            pssh_obj = PSSH(pssh.split(",")[-1])
+            cdm_session = self.cdm.open()
+            challenge = base64.b64encode(
+                self.cdm.get_license_challenge(cdm_session, pssh_obj)
+            ).decode()
+            license = self.apple_music_api.get_widevine_license(
+                track_id,
+                pssh,
+                challenge,
+            )
+            self.cdm.parse_license(cdm_session, license)
+            decryption_key = next(
+                i for i in self.cdm.get_keys(cdm_session) if i.type == "CONTENT"
+            ).key.hex()
+        finally:
+            self.cdm.close(cdm_session)
         return decryption_key
 
     def download(self, path: Path, stream_url: str):
         if self.download_mode == DownloadMode.YTDLP:
             self.download_ytdlp(path, stream_url)
         elif self.download_mode == DownloadMode.NM3U8DLRE:
             self.download_nm3u8dlre(path, stream_url)
```

### Comparing `gamdl-2.2.2/gamdl/downloader_music_video.py` & `gamdl-2.2.3/gamdl/downloader_music_video.py`

 * *Files identical despite different names*

### Comparing `gamdl-2.2.2/gamdl/downloader_post.py` & `gamdl-2.2.3/gamdl/downloader_post.py`

 * *Files identical despite different names*

### Comparing `gamdl-2.2.2/gamdl/downloader_song.py` & `gamdl-2.2.3/gamdl/downloader_song.py`

 * *Files identical despite different names*

### Comparing `gamdl-2.2.2/gamdl/downloader_song_legacy.py` & `gamdl-2.2.3/gamdl/downloader_song_legacy.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,32 +24,36 @@
             i for i in webplayback["assets"] if i["flavor"] == flavor
         )["URL"]
         m3u8_obj = m3u8.load(stream_info.stream_url)
         stream_info.pssh = m3u8_obj.keys[0].uri
         return stream_info
 
     def get_decryption_key(self, pssh: str, track_id: str) -> str:
-        widevine_pssh_data = WidevinePsshData()
-        widevine_pssh_data.algorithm = 1
-        widevine_pssh_data.key_ids.append(base64.b64decode(pssh.split(",")[1]))
-        pssh_obj = PSSH(widevine_pssh_data.SerializeToString())
-        cdm_session = self.downloader.cdm.open()
-        challenge = base64.b64encode(
-            self.downloader.cdm.get_license_challenge(cdm_session, pssh_obj)
-        ).decode()
-        license = self.downloader.apple_music_api.get_widevine_license(
-            track_id,
-            pssh,
-            challenge,
-        )
-        self.downloader.cdm.parse_license(cdm_session, license)
-        decryption_key = next(
-            i for i in self.downloader.cdm.get_keys(cdm_session) if i.type == "CONTENT"
-        ).key.hex()
-        self.downloader.cdm.close(cdm_session)
+        try:
+            widevine_pssh_data = WidevinePsshData()
+            widevine_pssh_data.algorithm = 1
+            widevine_pssh_data.key_ids.append(base64.b64decode(pssh.split(",")[1]))
+            pssh_obj = PSSH(widevine_pssh_data.SerializeToString())
+            cdm_session = self.downloader.cdm.open()
+            challenge = base64.b64encode(
+                self.downloader.cdm.get_license_challenge(cdm_session, pssh_obj)
+            ).decode()
+            license = self.downloader.apple_music_api.get_widevine_license(
+                track_id,
+                pssh,
+                challenge,
+            )
+            self.downloader.cdm.parse_license(cdm_session, license)
+            decryption_key = next(
+                i
+                for i in self.downloader.cdm.get_keys(cdm_session)
+                if i.type == "CONTENT"
+            ).key.hex()
+        finally:
+            self.downloader.cdm.close(cdm_session)
         return decryption_key
 
     def decrypt(
         self,
         encrypted_path: Path,
         decrypted_path: Path,
         decryption_key: str,
```

### Comparing `gamdl-2.2.2/gamdl/enums.py` & `gamdl-2.2.3/gamdl/enums.py`

 * *Files identical despite different names*

### Comparing `gamdl-2.2.2/gamdl/hardcoded_wvd.py` & `gamdl-2.2.3/gamdl/hardcoded_wvd.py`

 * *Files identical despite different names*

### Comparing `gamdl-2.2.2/gamdl/itunes_api.py` & `gamdl-2.2.3/gamdl/itunes_api.py`

 * *Files identical despite different names*

### Comparing `gamdl-2.2.2/pyproject.toml` & `gamdl-2.2.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gamdl-2.2.2/PKG-INFO` & `gamdl-2.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gamdl
-Version: 2.2.2
+Version: 2.2.3
 Summary: A Python CLI app for downloading Apple Music songs/music videos/albums/playlists/posts.
 Author: glomatico
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: ciso8601
 Requires-Dist: click
 Requires-Dist: inquirerpy
@@ -205,8 +205,7 @@
     * Highly unsupported by media players.
   
 ### Cover formats
 The following cover formats are available:
 * `jpg`
 * `png`
 
-
```

