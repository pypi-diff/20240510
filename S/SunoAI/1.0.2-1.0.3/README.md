# Comparing `tmp/sunoai-1.0.2.tar.gz` & `tmp/sunoai-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sunoai-1.0.2.tar", last modified: Fri May 10 08:08:20 2024, max compression
+gzip compressed data, was "sunoai-1.0.3.tar", last modified: Fri May 10 08:25:51 2024, max compression
```

## Comparing `sunoai-1.0.2.tar` & `sunoai-1.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 malithrukshan   (501) staff       (20)        0 2024-05-10 08:08:20.718530 sunoai-1.0.2/
--rw-r--r--   0 malithrukshan   (501) staff       (20)     1071 2024-05-08 13:39:56.000000 sunoai-1.0.2/LICENSE
--rw-r--r--   0 malithrukshan   (501) staff       (20)    15388 2024-05-10 08:08:20.718128 sunoai-1.0.2/PKG-INFO
--rw-r--r--   0 malithrukshan   (501) staff       (20)    14890 2024-05-10 08:00:19.000000 sunoai-1.0.2/README.md
-drwxr-xr-x   0 malithrukshan   (501) staff       (20)        0 2024-05-10 08:08:20.717891 sunoai-1.0.2/SunoAI.egg-info/
--rw-r--r--   0 malithrukshan   (501) staff       (20)    15388 2024-05-10 08:08:20.000000 sunoai-1.0.2/SunoAI.egg-info/PKG-INFO
--rw-r--r--   0 malithrukshan   (501) staff       (20)      234 2024-05-10 08:08:20.000000 sunoai-1.0.2/SunoAI.egg-info/SOURCES.txt
--rw-r--r--   0 malithrukshan   (501) staff       (20)        1 2024-05-10 08:08:20.000000 sunoai-1.0.2/SunoAI.egg-info/dependency_links.txt
--rw-r--r--   0 malithrukshan   (501) staff       (20)       18 2024-05-10 08:08:20.000000 sunoai-1.0.2/SunoAI.egg-info/requires.txt
--rw-r--r--   0 malithrukshan   (501) staff       (20)        5 2024-05-10 08:08:20.000000 sunoai-1.0.2/SunoAI.egg-info/top_level.txt
--rw-r--r--   0 malithrukshan   (501) staff       (20)       38 2024-05-10 08:08:20.718572 sunoai-1.0.2/setup.cfg
--rw-r--r--   0 malithrukshan   (501) staff       (20)      757 2024-05-10 08:08:00.000000 sunoai-1.0.2/setup.py
-drwxr-xr-x   0 malithrukshan   (501) staff       (20)        0 2024-05-10 08:08:20.717507 sunoai-1.0.2/suno/
--rw-r--r--   0 malithrukshan   (501) staff       (20)      176 2024-05-10 08:07:06.000000 sunoai-1.0.2/suno/__init__.py
--rw-r--r--   0 malithrukshan   (501) staff       (20)     5160 2024-05-07 19:51:06.000000 sunoai-1.0.2/suno/models.py
--rw-r--r--   0 malithrukshan   (501) staff       (20)    10199 2024-05-10 08:06:27.000000 sunoai-1.0.2/suno/suno.py
--rw-r--r--   0 malithrukshan   (501) staff       (20)     1108 2024-05-07 19:51:51.000000 sunoai-1.0.2/suno/utils.py
+drwxr-xr-x   0 malithrukshan   (501) staff       (20)        0 2024-05-10 08:25:51.509300 sunoai-1.0.3/
+-rw-r--r--   0 malithrukshan   (501) staff       (20)     1071 2024-05-08 13:39:56.000000 sunoai-1.0.3/LICENSE
+-rw-r--r--   0 malithrukshan   (501) staff       (20)    15388 2024-05-10 08:25:51.508917 sunoai-1.0.3/PKG-INFO
+-rw-r--r--   0 malithrukshan   (501) staff       (20)    14890 2024-05-10 08:00:19.000000 sunoai-1.0.3/README.md
+drwxr-xr-x   0 malithrukshan   (501) staff       (20)        0 2024-05-10 08:25:51.508676 sunoai-1.0.3/SunoAI.egg-info/
+-rw-r--r--   0 malithrukshan   (501) staff       (20)    15388 2024-05-10 08:25:51.000000 sunoai-1.0.3/SunoAI.egg-info/PKG-INFO
+-rw-r--r--   0 malithrukshan   (501) staff       (20)      234 2024-05-10 08:25:51.000000 sunoai-1.0.3/SunoAI.egg-info/SOURCES.txt
+-rw-r--r--   0 malithrukshan   (501) staff       (20)        1 2024-05-10 08:25:51.000000 sunoai-1.0.3/SunoAI.egg-info/dependency_links.txt
+-rw-r--r--   0 malithrukshan   (501) staff       (20)       18 2024-05-10 08:25:51.000000 sunoai-1.0.3/SunoAI.egg-info/requires.txt
+-rw-r--r--   0 malithrukshan   (501) staff       (20)        5 2024-05-10 08:25:51.000000 sunoai-1.0.3/SunoAI.egg-info/top_level.txt
+-rw-r--r--   0 malithrukshan   (501) staff       (20)       38 2024-05-10 08:25:51.509341 sunoai-1.0.3/setup.cfg
+-rw-r--r--   0 malithrukshan   (501) staff       (20)      757 2024-05-10 08:14:51.000000 sunoai-1.0.3/setup.py
+drwxr-xr-x   0 malithrukshan   (501) staff       (20)        0 2024-05-10 08:25:51.508252 sunoai-1.0.3/suno/
+-rw-r--r--   0 malithrukshan   (501) staff       (20)      176 2024-05-10 08:25:23.000000 sunoai-1.0.3/suno/__init__.py
+-rw-r--r--   0 malithrukshan   (501) staff       (20)     5160 2024-05-07 19:51:06.000000 sunoai-1.0.3/suno/models.py
+-rw-r--r--   0 malithrukshan   (501) staff       (20)    10612 2024-05-10 08:24:46.000000 sunoai-1.0.3/suno/suno.py
+-rw-r--r--   0 malithrukshan   (501) staff       (20)     1108 2024-05-07 19:51:51.000000 sunoai-1.0.3/suno/utils.py
```

### Comparing `sunoai-1.0.2/LICENSE` & `sunoai-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sunoai-1.0.2/PKG-INFO` & `sunoai-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SunoAI
-Version: 1.0.2
+Version: 1.0.3
 Summary: Python API for interacting with the Suno AI music generator - Unofficial
 Home-page: https://github.com/Malith-Rukshan/Suno-API
 Author: Malith Rukshan
 Author-email: singledeveloper.lk@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: SunoAI Version: 1.0.2 Summary: Python API for
+Metadata-Version: 2.1 Name: SunoAI Version: 1.0.3 Summary: Python API for
 interacting with the Suno AI music generator - Unofficial Home-page: https://
 github.com/Malith-Rukshan/Suno-API Author: Malith Rukshan Author-email:
 singledeveloper.lk@gmail.com License: MIT Classifier: Programming Language ::
 Python :: 3 Classifier: License :: OSI Approved :: MIT License Requires-Python:
 >=3.7 Description-Content-Type: text/markdown License-File: LICENSE Requires-
 Dist: requests Requires-Dist: pydantic
    [https://raw.githubusercontent.com/Malith-Rukshan/Suno-API/main/Logo.png]
```

### Comparing `sunoai-1.0.2/README.md` & `sunoai-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `sunoai-1.0.2/SunoAI.egg-info/PKG-INFO` & `sunoai-1.0.3/SunoAI.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SunoAI
-Version: 1.0.2
+Version: 1.0.3
 Summary: Python API for interacting with the Suno AI music generator - Unofficial
 Home-page: https://github.com/Malith-Rukshan/Suno-API
 Author: Malith Rukshan
 Author-email: singledeveloper.lk@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: SunoAI Version: 1.0.2 Summary: Python API for
+Metadata-Version: 2.1 Name: SunoAI Version: 1.0.3 Summary: Python API for
 interacting with the Suno AI music generator - Unofficial Home-page: https://
 github.com/Malith-Rukshan/Suno-API Author: Malith Rukshan Author-email:
 singledeveloper.lk@gmail.com License: MIT Classifier: Programming Language ::
 Python :: 3 Classifier: License :: OSI Approved :: MIT License Requires-Python:
 >=3.7 Description-Content-Type: text/markdown License-File: LICENSE Requires-
 Dist: requests Requires-Dist: pydantic
    [https://raw.githubusercontent.com/Malith-Rukshan/Suno-API/main/Logo.png]
```

### Comparing `sunoai-1.0.2/setup.py` & `sunoai-1.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='SunoAI', 
-    version='1.0.2',
+    version='1.0.3',
     description='Python API for interacting with the Suno AI music generator - Unofficial',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/Malith-Rukshan/Suno-API',
     author='Malith Rukshan',
     author_email='singledeveloper.lk@gmail.com',
     license='MIT',
```

### Comparing `sunoai-1.0.2/suno/models.py` & `sunoai-1.0.3/suno/models.py`

 * *Files identical despite different names*

### Comparing `sunoai-1.0.2/suno/suno.py` & `sunoai-1.0.3/suno/suno.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,14 +72,22 @@
             time.sleep(random.uniform(1, 2))
 
         new_token = renew_response.json()['jwt']
         self.current_token = new_token
         # Set New Token to Headers
         self.client.headers['Authorization'] = f"Bearer {new_token}"
 
+    def _cehck_error(self, response):
+        try:
+            resp = response.json()
+            if resp['detail']:
+                raise Exception(resp['detail'])
+        except:
+            pass
+
     # Generate Songs
     def generate(self, prompt, is_custom, tags="", title="", make_instrumental=False, wait_audio=False) -> List[Clip]:
         """
         Generate songs based on the provided parameters and optionally wait for the audio to be ready.
 
         Parameters:
         - prompt (str): If is_custom=True, this should be the lyrics of the song. If False, it should be a brief description of what the song should be about.
@@ -106,14 +114,16 @@
         else:
             payload["gpt_description_prompt"] = prompt
 
         response = self.client.post(
             f"{Suno.BASE_URL}/api/generate/v2/", json=payload)
         logger.info(response.text)
 
+        self._cehck_error(response)
+
         if response.status_code != 200:
             logger.error("Audio Generate Failed ⁉️")
             raise Exception(f"Error response: {response.text}")
 
         song_ids = [audio['id'] for audio in response.json()['clips']]
         if wait_audio:
             return self._wait_for_audio(song_ids)
@@ -124,21 +134,23 @@
 
     def _wait_for_audio(self, song_ids):
         """Helper method to wait for audio processing to complete."""
         start_time = time.time()
         last_clips = []
         time.sleep(random.uniform(10, 20))  # Wait
         while time.time() - start_time < 200:  # Timeout after 200 seconds
-            clips = self.get_songs(song_ids)
-            all_completed = all(
-                audio.status in ['streaming', 'complete'] for audio in clips)
-            if all_completed:
-                logger.info("Generated Audio Successfully ✅")
-                return clips
-            last_clips = clips
+            try:
+                clips = self.get_songs(song_ids)
+                all_completed = all(
+                    audio.status in ['streaming', 'complete'] for audio in clips)
+                if all_completed:
+                    logger.info("Generated Audio Successfully ✅")
+                    return clips
+                last_clips = clips
+            except:pass
             time.sleep(random.uniform(3, 6))  # Wait with variation
             self._keep_alive(True)
         logger.info("Generated Audio Successfully ✅")
         return last_clips
 
     def get_songs(self, song_ids: str = None) -> List[Clip]:
         """
@@ -157,14 +169,15 @@
         self._keep_alive()  # Ensure session is active
         url = f"{Suno.BASE_URL}/api/feed/"
         if song_ids:
             url += f"?ids={song_ids}"
         logger.info("Getting Songs Info...")
         response = self.client.get(url)  # Call API
         logger.info(response.text)
+        self._cehck_error(response)
         return response_to_clips(response.json())
 
     def get_song(self, id: str) -> Clip:
         """
         Retrieve a single song by its ID.
 
         Parameters:
@@ -174,23 +187,25 @@
         Clip: A Clip object containing details about the song, such as the audio URL, song status, and other metadata.
         """
         self._keep_alive()  # Ensure session is active
         logger.info("Getting Song Info...")
         response = self.client.get(
             f"{Suno.BASE_URL}/api/feed/?ids={id}")  # Call API
         logger.info(response.text)
+        self._cehck_error(response)
         return create_clip_from_data(response.json()[0])
 
     def get_credits(self) -> CreditsInfo:
         """Retrieve current billing and credits information."""
         self._keep_alive()  # Ensure session is active
         logger.info("Credits Info...")
         response = self.client.get(
             f"{Suno.BASE_URL}/api/billing/info/")  # Call API
         logger.info(response.text)
+        self._cehck_error(response)
         if response.status_code == 200:
             data = response.json()
             result = {
                 "credits_left": data["total_credits_left"],
                 "period": data["period"],
                 "monthly_limit": data["monthly_limit"],
                 "monthly_usage": data["monthly_usage"],
```

### Comparing `sunoai-1.0.2/suno/utils.py` & `sunoai-1.0.3/suno/utils.py`

 * *Files identical despite different names*

