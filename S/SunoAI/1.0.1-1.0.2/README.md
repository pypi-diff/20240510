# Comparing `tmp/sunoai-1.0.1.tar.gz` & `tmp/sunoai-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sunoai-1.0.1.tar", last modified: Wed May  8 14:45:42 2024, max compression
+gzip compressed data, was "sunoai-1.0.2.tar", last modified: Fri May 10 08:08:20 2024, max compression
```

## Comparing `sunoai-1.0.1.tar` & `sunoai-1.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 malithrukshan   (501) staff       (20)        0 2024-05-08 14:45:42.164751 sunoai-1.0.1/
--rw-r--r--   0 malithrukshan   (501) staff       (20)     1071 2024-05-08 13:39:56.000000 sunoai-1.0.1/LICENSE
--rw-r--r--   0 malithrukshan   (501) staff       (20)    15230 2024-05-08 14:45:42.164457 sunoai-1.0.1/PKG-INFO
--rw-r--r--   0 malithrukshan   (501) staff       (20)    14732 2024-05-08 14:37:59.000000 sunoai-1.0.1/README.md
-drwxr-xr-x   0 malithrukshan   (501) staff       (20)        0 2024-05-08 14:45:42.164225 sunoai-1.0.1/SunoAI.egg-info/
--rw-r--r--   0 malithrukshan   (501) staff       (20)    15230 2024-05-08 14:45:42.000000 sunoai-1.0.1/SunoAI.egg-info/PKG-INFO
--rw-r--r--   0 malithrukshan   (501) staff       (20)      234 2024-05-08 14:45:42.000000 sunoai-1.0.1/SunoAI.egg-info/SOURCES.txt
--rw-r--r--   0 malithrukshan   (501) staff       (20)        1 2024-05-08 14:45:42.000000 sunoai-1.0.1/SunoAI.egg-info/dependency_links.txt
--rw-r--r--   0 malithrukshan   (501) staff       (20)       18 2024-05-08 14:45:42.000000 sunoai-1.0.1/SunoAI.egg-info/requires.txt
--rw-r--r--   0 malithrukshan   (501) staff       (20)        5 2024-05-08 14:45:42.000000 sunoai-1.0.1/SunoAI.egg-info/top_level.txt
--rw-r--r--   0 malithrukshan   (501) staff       (20)       38 2024-05-08 14:45:42.164795 sunoai-1.0.1/setup.cfg
--rw-r--r--   0 malithrukshan   (501) staff       (20)      757 2024-05-08 14:39:02.000000 sunoai-1.0.1/setup.py
-drwxr-xr-x   0 malithrukshan   (501) staff       (20)        0 2024-05-08 14:45:42.163703 sunoai-1.0.1/suno/
--rw-r--r--   0 malithrukshan   (501) staff       (20)      176 2024-05-08 14:38:57.000000 sunoai-1.0.1/suno/__init__.py
--rw-r--r--   0 malithrukshan   (501) staff       (20)     5160 2024-05-07 19:51:06.000000 sunoai-1.0.1/suno/models.py
--rw-r--r--   0 malithrukshan   (501) staff       (20)    10015 2024-05-07 19:51:59.000000 sunoai-1.0.1/suno/suno.py
--rw-r--r--   0 malithrukshan   (501) staff       (20)     1108 2024-05-07 19:51:51.000000 sunoai-1.0.1/suno/utils.py
+drwxr-xr-x   0 malithrukshan   (501) staff       (20)        0 2024-05-10 08:08:20.718530 sunoai-1.0.2/
+-rw-r--r--   0 malithrukshan   (501) staff       (20)     1071 2024-05-08 13:39:56.000000 sunoai-1.0.2/LICENSE
+-rw-r--r--   0 malithrukshan   (501) staff       (20)    15388 2024-05-10 08:08:20.718128 sunoai-1.0.2/PKG-INFO
+-rw-r--r--   0 malithrukshan   (501) staff       (20)    14890 2024-05-10 08:00:19.000000 sunoai-1.0.2/README.md
+drwxr-xr-x   0 malithrukshan   (501) staff       (20)        0 2024-05-10 08:08:20.717891 sunoai-1.0.2/SunoAI.egg-info/
+-rw-r--r--   0 malithrukshan   (501) staff       (20)    15388 2024-05-10 08:08:20.000000 sunoai-1.0.2/SunoAI.egg-info/PKG-INFO
+-rw-r--r--   0 malithrukshan   (501) staff       (20)      234 2024-05-10 08:08:20.000000 sunoai-1.0.2/SunoAI.egg-info/SOURCES.txt
+-rw-r--r--   0 malithrukshan   (501) staff       (20)        1 2024-05-10 08:08:20.000000 sunoai-1.0.2/SunoAI.egg-info/dependency_links.txt
+-rw-r--r--   0 malithrukshan   (501) staff       (20)       18 2024-05-10 08:08:20.000000 sunoai-1.0.2/SunoAI.egg-info/requires.txt
+-rw-r--r--   0 malithrukshan   (501) staff       (20)        5 2024-05-10 08:08:20.000000 sunoai-1.0.2/SunoAI.egg-info/top_level.txt
+-rw-r--r--   0 malithrukshan   (501) staff       (20)       38 2024-05-10 08:08:20.718572 sunoai-1.0.2/setup.cfg
+-rw-r--r--   0 malithrukshan   (501) staff       (20)      757 2024-05-10 08:08:00.000000 sunoai-1.0.2/setup.py
+drwxr-xr-x   0 malithrukshan   (501) staff       (20)        0 2024-05-10 08:08:20.717507 sunoai-1.0.2/suno/
+-rw-r--r--   0 malithrukshan   (501) staff       (20)      176 2024-05-10 08:07:06.000000 sunoai-1.0.2/suno/__init__.py
+-rw-r--r--   0 malithrukshan   (501) staff       (20)     5160 2024-05-07 19:51:06.000000 sunoai-1.0.2/suno/models.py
+-rw-r--r--   0 malithrukshan   (501) staff       (20)    10199 2024-05-10 08:06:27.000000 sunoai-1.0.2/suno/suno.py
+-rw-r--r--   0 malithrukshan   (501) staff       (20)     1108 2024-05-07 19:51:51.000000 sunoai-1.0.2/suno/utils.py
```

### Comparing `sunoai-1.0.1/LICENSE` & `sunoai-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sunoai-1.0.1/PKG-INFO` & `sunoai-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SunoAI
-Version: 1.0.1
+Version: 1.0.2
 Summary: Python API for interacting with the Suno AI music generator - Unofficial
 Home-page: https://github.com/Malith-Rukshan/Suno-API
 Author: Malith Rukshan
 Author-email: singledeveloper.lk@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -83,14 +83,15 @@
 ### Deploy on PasS
 
 Set `SUNO_COOKIE` as an Environmental variable before deploy. -  [Instructions](#-prerequisites)
 
 [![Deploy with heroku](https://www.herokucdn.com/deploy/button.svg)](https://heroku.com/deploy)
 [![Deploy to Netlify](https://www.netlify.com/img/deploy/button.svg)](https://app.netlify.com/start/deploy?repository=https://github.com/Malith-Rukshan/Suno-API)
 
+[![Deploy on Railway](https://railway.app/button.svg)](https://railway.app/template/IdlBP8?referralCode=jC4ZQ_)
 [![Deploy to Render](https://render.com/images/deploy-to-render-button.svg)](https://render.com/deploy)
 </br>
 
 ### Deploy on Local or VPS
 
 ```
 export SUNO_COOKIE="YOUR_COOKIE_HERE"
@@ -105,19 +106,20 @@
 
 **⚡️ Quick Start :**
 ```
 import suno
 client = suno.Suno(cookie='YOUR_COOKIE_HERE')
 
 # Generate a song
-song = client.generate(prompt="A serene landscape", wait_audio=True)
+songs = client.generate(prompt="A serene landscape", is_custom=False, wait_audio=True)
 
-# Download generated song
-file_path = client.download(song=song)
-print(f"Song downloaded to: {file_path}")
+# Download generated songs
+for song in songs:
+    file_path = client.download(song=song)
+    print(f"Song downloaded to: {file_path}")
 ```
 
 ### 📚 Library Methods
 
 `generate()`
 - <b>Arguments</b>:
   - prompt (str): Description or lyrics for the song.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: SunoAI Version: 1.0.1 Summary: Python API for
+Metadata-Version: 2.1 Name: SunoAI Version: 1.0.2 Summary: Python API for
 interacting with the Suno AI music generator - Unofficial Home-page: https://
 github.com/Malith-Rukshan/Suno-API Author: Malith Rukshan Author-email:
 singledeveloper.lk@gmail.com License: MIT Classifier: Programming Language ::
 Python :: 3 Classifier: License :: OSI Approved :: MIT License Requires-Python:
 >=3.7 Description-Content-Type: text/markdown License-File: LICENSE Requires-
 Dist: requests Requires-Dist: pydantic
    [https://raw.githubusercontent.com/Malith-Rukshan/Suno-API/main/Logo.png]
@@ -40,27 +40,29 @@
 (cookie='YOUR_COOKIE_HERE') ``` ## ð¾ Installation Install the library using
 pip: ``` pip install SunoAI ``` _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_P_y_P_i_-_L_i_b_r_a_r_y_-
 _1_c_d_7_6_0_?_l_o_g_o_=_p_y_p_i_&_s_t_y_l_e_=_f_l_a_t_]## ð Deployment - REST API ### Deploy on PasS
 Set `SUNO_COOKIE` as an Environmental variable before deploy. - [Instructions]
 (#-prerequisites) [![Deploy with heroku](https://www.herokucdn.com/deploy/
 button.svg)](https://heroku.com/deploy) [![Deploy to Netlify](https://
 www.netlify.com/img/deploy/button.svg)](https://app.netlify.com/start/
-deploy?repository=https://github.com/Malith-Rukshan/Suno-API) [![Deploy to
-Render](https://render.com/images/deploy-to-render-button.svg)](https://
-render.com/deploy) ### Deploy on Local or VPS ``` export
-SUNO_COOKIE="YOUR_COOKIE_HERE" git clone git@github.com:Malith-Rukshan/Suno-
-API.git pip3 install -r requirements.txt cd Suno-API fastapi run api.py --port
-8080 ``` ð Available at : http://127.0.0.1:8080 ## ð ï¸ Usage **â¡ï¸
-Quick Start :** ``` import suno client = suno.Suno(cookie='YOUR_COOKIE_HERE') #
-Generate a song song = client.generate(prompt="A serene landscape",
-wait_audio=True) # Download generated song file_path = client.download
-(song=song) print(f"Song downloaded to: {file_path}") ``` ### ð Library
-Methods `generate()` - AArrgguummeennttss: - prompt (str): Description or lyrics for the
-song. - is_custom (bool): Determines whether to use custom lyrics (True) or a
-description (False). - tags (Optional[str]): Describes desired voice type or
+deploy?repository=https://github.com/Malith-Rukshan/Suno-API) [![Deploy on
+Railway](https://railway.app/button.svg)](https://railway.app/template/
+IdlBP8?referralCode=jC4ZQ_) [![Deploy to Render](https://render.com/images/
+deploy-to-render-button.svg)](https://render.com/deploy) ### Deploy on Local or
+VPS ``` export SUNO_COOKIE="YOUR_COOKIE_HERE" git clone git@github.com:Malith-
+Rukshan/Suno-API.git pip3 install -r requirements.txt cd Suno-API fastapi run
+api.py --port 8080 ``` ð Available at : http://127.0.0.1:8080 ## ð ï¸
+Usage **â¡ï¸ Quick Start :** ``` import suno client = suno.Suno
+(cookie='YOUR_COOKIE_HERE') # Generate a song songs = client.generate(prompt="A
+serene landscape", is_custom=False, wait_audio=True) # Download generated songs
+for song in songs: file_path = client.download(song=song) print(f"Song
+downloaded to: {file_path}") ``` ### ð Library Methods `generate()` -
+AArrgguummeennttss: - prompt (str): Description or lyrics for the song. - is_custom
+(bool): Determines whether to use custom lyrics (True) or a description
+(False). - tags (Optional[str]): Describes desired voice type or
 characteristics. - title (Optional[str]): Title for the generated music. -
 make_instrumental (Optional[bool]): Generates an instrumental version if True.
 - wait_audio (bool): Waits until the audio URLs are ready if True. - RReettuurrnnss: A
 list of `Clip` objects containing song data with IDs. - EExxaammppllee:: - **By
 Description** ``` clips = client.generate( prompt="A peaceful melody reflecting
 a serene landscape", is_custom=False, wait_audio=True ) print(clips) ``` - **By
 Lyrics - Custom** ``` clips = client.generate( prompt="I found a love, for
```

### Comparing `sunoai-1.0.1/README.md` & `sunoai-1.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -67,14 +67,15 @@
 ### Deploy on PasS
 
 Set `SUNO_COOKIE` as an Environmental variable before deploy. -  [Instructions](#-prerequisites)
 
 [![Deploy with heroku](https://www.herokucdn.com/deploy/button.svg)](https://heroku.com/deploy)
 [![Deploy to Netlify](https://www.netlify.com/img/deploy/button.svg)](https://app.netlify.com/start/deploy?repository=https://github.com/Malith-Rukshan/Suno-API)
 
+[![Deploy on Railway](https://railway.app/button.svg)](https://railway.app/template/IdlBP8?referralCode=jC4ZQ_)
 [![Deploy to Render](https://render.com/images/deploy-to-render-button.svg)](https://render.com/deploy)
 </br>
 
 ### Deploy on Local or VPS
 
 ```
 export SUNO_COOKIE="YOUR_COOKIE_HERE"
@@ -89,19 +90,20 @@
 
 **⚡️ Quick Start :**
 ```
 import suno
 client = suno.Suno(cookie='YOUR_COOKIE_HERE')
 
 # Generate a song
-song = client.generate(prompt="A serene landscape", wait_audio=True)
+songs = client.generate(prompt="A serene landscape", is_custom=False, wait_audio=True)
 
-# Download generated song
-file_path = client.download(song=song)
-print(f"Song downloaded to: {file_path}")
+# Download generated songs
+for song in songs:
+    file_path = client.download(song=song)
+    print(f"Song downloaded to: {file_path}")
 ```
 
 ### 📚 Library Methods
 
 `generate()`
 - <b>Arguments</b>:
   - prompt (str): Description or lyrics for the song.
```

#### html2text {}

```diff
@@ -33,27 +33,29 @@
 (cookie='YOUR_COOKIE_HERE') ``` ## ð¾ Installation Install the library using
 pip: ``` pip install SunoAI ``` _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_P_y_P_i_-_L_i_b_r_a_r_y_-
 _1_c_d_7_6_0_?_l_o_g_o_=_p_y_p_i_&_s_t_y_l_e_=_f_l_a_t_]## ð Deployment - REST API ### Deploy on PasS
 Set `SUNO_COOKIE` as an Environmental variable before deploy. - [Instructions]
 (#-prerequisites) [![Deploy with heroku](https://www.herokucdn.com/deploy/
 button.svg)](https://heroku.com/deploy) [![Deploy to Netlify](https://
 www.netlify.com/img/deploy/button.svg)](https://app.netlify.com/start/
-deploy?repository=https://github.com/Malith-Rukshan/Suno-API) [![Deploy to
-Render](https://render.com/images/deploy-to-render-button.svg)](https://
-render.com/deploy) ### Deploy on Local or VPS ``` export
-SUNO_COOKIE="YOUR_COOKIE_HERE" git clone git@github.com:Malith-Rukshan/Suno-
-API.git pip3 install -r requirements.txt cd Suno-API fastapi run api.py --port
-8080 ``` ð Available at : http://127.0.0.1:8080 ## ð ï¸ Usage **â¡ï¸
-Quick Start :** ``` import suno client = suno.Suno(cookie='YOUR_COOKIE_HERE') #
-Generate a song song = client.generate(prompt="A serene landscape",
-wait_audio=True) # Download generated song file_path = client.download
-(song=song) print(f"Song downloaded to: {file_path}") ``` ### ð Library
-Methods `generate()` - AArrgguummeennttss: - prompt (str): Description or lyrics for the
-song. - is_custom (bool): Determines whether to use custom lyrics (True) or a
-description (False). - tags (Optional[str]): Describes desired voice type or
+deploy?repository=https://github.com/Malith-Rukshan/Suno-API) [![Deploy on
+Railway](https://railway.app/button.svg)](https://railway.app/template/
+IdlBP8?referralCode=jC4ZQ_) [![Deploy to Render](https://render.com/images/
+deploy-to-render-button.svg)](https://render.com/deploy) ### Deploy on Local or
+VPS ``` export SUNO_COOKIE="YOUR_COOKIE_HERE" git clone git@github.com:Malith-
+Rukshan/Suno-API.git pip3 install -r requirements.txt cd Suno-API fastapi run
+api.py --port 8080 ``` ð Available at : http://127.0.0.1:8080 ## ð ï¸
+Usage **â¡ï¸ Quick Start :** ``` import suno client = suno.Suno
+(cookie='YOUR_COOKIE_HERE') # Generate a song songs = client.generate(prompt="A
+serene landscape", is_custom=False, wait_audio=True) # Download generated songs
+for song in songs: file_path = client.download(song=song) print(f"Song
+downloaded to: {file_path}") ``` ### ð Library Methods `generate()` -
+AArrgguummeennttss: - prompt (str): Description or lyrics for the song. - is_custom
+(bool): Determines whether to use custom lyrics (True) or a description
+(False). - tags (Optional[str]): Describes desired voice type or
 characteristics. - title (Optional[str]): Title for the generated music. -
 make_instrumental (Optional[bool]): Generates an instrumental version if True.
 - wait_audio (bool): Waits until the audio URLs are ready if True. - RReettuurrnnss: A
 list of `Clip` objects containing song data with IDs. - EExxaammppllee:: - **By
 Description** ``` clips = client.generate( prompt="A peaceful melody reflecting
 a serene landscape", is_custom=False, wait_audio=True ) print(clips) ``` - **By
 Lyrics - Custom** ``` clips = client.generate( prompt="I found a love, for
```

### Comparing `sunoai-1.0.1/SunoAI.egg-info/PKG-INFO` & `sunoai-1.0.2/SunoAI.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SunoAI
-Version: 1.0.1
+Version: 1.0.2
 Summary: Python API for interacting with the Suno AI music generator - Unofficial
 Home-page: https://github.com/Malith-Rukshan/Suno-API
 Author: Malith Rukshan
 Author-email: singledeveloper.lk@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -83,14 +83,15 @@
 ### Deploy on PasS
 
 Set `SUNO_COOKIE` as an Environmental variable before deploy. -  [Instructions](#-prerequisites)
 
 [![Deploy with heroku](https://www.herokucdn.com/deploy/button.svg)](https://heroku.com/deploy)
 [![Deploy to Netlify](https://www.netlify.com/img/deploy/button.svg)](https://app.netlify.com/start/deploy?repository=https://github.com/Malith-Rukshan/Suno-API)
 
+[![Deploy on Railway](https://railway.app/button.svg)](https://railway.app/template/IdlBP8?referralCode=jC4ZQ_)
 [![Deploy to Render](https://render.com/images/deploy-to-render-button.svg)](https://render.com/deploy)
 </br>
 
 ### Deploy on Local or VPS
 
 ```
 export SUNO_COOKIE="YOUR_COOKIE_HERE"
@@ -105,19 +106,20 @@
 
 **⚡️ Quick Start :**
 ```
 import suno
 client = suno.Suno(cookie='YOUR_COOKIE_HERE')
 
 # Generate a song
-song = client.generate(prompt="A serene landscape", wait_audio=True)
+songs = client.generate(prompt="A serene landscape", is_custom=False, wait_audio=True)
 
-# Download generated song
-file_path = client.download(song=song)
-print(f"Song downloaded to: {file_path}")
+# Download generated songs
+for song in songs:
+    file_path = client.download(song=song)
+    print(f"Song downloaded to: {file_path}")
 ```
 
 ### 📚 Library Methods
 
 `generate()`
 - <b>Arguments</b>:
   - prompt (str): Description or lyrics for the song.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: SunoAI Version: 1.0.1 Summary: Python API for
+Metadata-Version: 2.1 Name: SunoAI Version: 1.0.2 Summary: Python API for
 interacting with the Suno AI music generator - Unofficial Home-page: https://
 github.com/Malith-Rukshan/Suno-API Author: Malith Rukshan Author-email:
 singledeveloper.lk@gmail.com License: MIT Classifier: Programming Language ::
 Python :: 3 Classifier: License :: OSI Approved :: MIT License Requires-Python:
 >=3.7 Description-Content-Type: text/markdown License-File: LICENSE Requires-
 Dist: requests Requires-Dist: pydantic
    [https://raw.githubusercontent.com/Malith-Rukshan/Suno-API/main/Logo.png]
@@ -40,27 +40,29 @@
 (cookie='YOUR_COOKIE_HERE') ``` ## ð¾ Installation Install the library using
 pip: ``` pip install SunoAI ``` _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_P_y_P_i_-_L_i_b_r_a_r_y_-
 _1_c_d_7_6_0_?_l_o_g_o_=_p_y_p_i_&_s_t_y_l_e_=_f_l_a_t_]## ð Deployment - REST API ### Deploy on PasS
 Set `SUNO_COOKIE` as an Environmental variable before deploy. - [Instructions]
 (#-prerequisites) [![Deploy with heroku](https://www.herokucdn.com/deploy/
 button.svg)](https://heroku.com/deploy) [![Deploy to Netlify](https://
 www.netlify.com/img/deploy/button.svg)](https://app.netlify.com/start/
-deploy?repository=https://github.com/Malith-Rukshan/Suno-API) [![Deploy to
-Render](https://render.com/images/deploy-to-render-button.svg)](https://
-render.com/deploy) ### Deploy on Local or VPS ``` export
-SUNO_COOKIE="YOUR_COOKIE_HERE" git clone git@github.com:Malith-Rukshan/Suno-
-API.git pip3 install -r requirements.txt cd Suno-API fastapi run api.py --port
-8080 ``` ð Available at : http://127.0.0.1:8080 ## ð ï¸ Usage **â¡ï¸
-Quick Start :** ``` import suno client = suno.Suno(cookie='YOUR_COOKIE_HERE') #
-Generate a song song = client.generate(prompt="A serene landscape",
-wait_audio=True) # Download generated song file_path = client.download
-(song=song) print(f"Song downloaded to: {file_path}") ``` ### ð Library
-Methods `generate()` - AArrgguummeennttss: - prompt (str): Description or lyrics for the
-song. - is_custom (bool): Determines whether to use custom lyrics (True) or a
-description (False). - tags (Optional[str]): Describes desired voice type or
+deploy?repository=https://github.com/Malith-Rukshan/Suno-API) [![Deploy on
+Railway](https://railway.app/button.svg)](https://railway.app/template/
+IdlBP8?referralCode=jC4ZQ_) [![Deploy to Render](https://render.com/images/
+deploy-to-render-button.svg)](https://render.com/deploy) ### Deploy on Local or
+VPS ``` export SUNO_COOKIE="YOUR_COOKIE_HERE" git clone git@github.com:Malith-
+Rukshan/Suno-API.git pip3 install -r requirements.txt cd Suno-API fastapi run
+api.py --port 8080 ``` ð Available at : http://127.0.0.1:8080 ## ð ï¸
+Usage **â¡ï¸ Quick Start :** ``` import suno client = suno.Suno
+(cookie='YOUR_COOKIE_HERE') # Generate a song songs = client.generate(prompt="A
+serene landscape", is_custom=False, wait_audio=True) # Download generated songs
+for song in songs: file_path = client.download(song=song) print(f"Song
+downloaded to: {file_path}") ``` ### ð Library Methods `generate()` -
+AArrgguummeennttss: - prompt (str): Description or lyrics for the song. - is_custom
+(bool): Determines whether to use custom lyrics (True) or a description
+(False). - tags (Optional[str]): Describes desired voice type or
 characteristics. - title (Optional[str]): Title for the generated music. -
 make_instrumental (Optional[bool]): Generates an instrumental version if True.
 - wait_audio (bool): Waits until the audio URLs are ready if True. - RReettuurrnnss: A
 list of `Clip` objects containing song data with IDs. - EExxaammppllee:: - **By
 Description** ``` clips = client.generate( prompt="A peaceful melody reflecting
 a serene landscape", is_custom=False, wait_audio=True ) print(clips) ``` - **By
 Lyrics - Custom** ``` clips = client.generate( prompt="I found a love, for
```

### Comparing `sunoai-1.0.1/setup.py` & `sunoai-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='SunoAI', 
-    version='1.0.1',
+    version='1.0.2',
     description='Python API for interacting with the Suno AI music generator - Unofficial',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/Malith-Rukshan/Suno-API',
     author='Malith Rukshan',
     author_email='singledeveloper.lk@gmail.com',
     license='MIT',
```

### Comparing `sunoai-1.0.1/suno/models.py` & `sunoai-1.0.2/suno/models.py`

 * *Files identical despite different names*

### Comparing `sunoai-1.0.1/suno/suno.py` & `sunoai-1.0.2/suno/suno.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from typing import List, Optional
 import requests
 
 from .models import Clip, CreditsInfo
 from .utils import create_clip_from_data, response_to_clips, generate_fake_useragent
 
 # Setup basic logging configuration
-logger = logging.getLogger(__name__)
+logger = logging.getLogger("SunoAI")
 logging.basicConfig(level=logging.INFO)
 
 # Fetch the cookie from environment variables; used for authentication
 COOKIE = os.getenv("SUNO_COOKIE", "")
 
 
 class Suno():
@@ -73,23 +73,23 @@
 
         new_token = renew_response.json()['jwt']
         self.current_token = new_token
         # Set New Token to Headers
         self.client.headers['Authorization'] = f"Bearer {new_token}"
 
     # Generate Songs
-    def generate(self, prompt, is_custom, tags=None, title=None, make_instrumental=False, wait_audio=False) -> List[Clip]:
+    def generate(self, prompt, is_custom, tags="", title="", make_instrumental=False, wait_audio=False) -> List[Clip]:
         """
         Generate songs based on the provided parameters and optionally wait for the audio to be ready.
 
         Parameters:
         - prompt (str): If is_custom=True, this should be the lyrics of the song. If False, it should be a brief description of what the song should be about.
         - is_custom (bool): Determines whether the song should be generated from custom lyrics (True) or from a description (False).
-        - tags (Optional[str]): Describes the desired voice type or characteristics (e.g., "English male voice"). Default is None.
-        - title (Optional[str]): The title for the generated music. Default is None.
+        - tags (Optional[str]): Describes the desired voice type or characteristics (e.g., "English male voice"). Default is "".
+        - title (Optional[str]): The title for the generated music. Default is "".
         - make_instrumental (Optional[bool]): If True, generates an instrumental version of the track. Default is False.
         - wait_audio (bool): If True, waits until the audio URLs are ready and returns them. If False, returns the IDs of the songs being processed, which can be used to fetch the songs later using get_song.
 
         Returns:
         List[Clip]: A list of Clip objects containing either song IDs or complete song data, depending on the 'wait_audio' parameter.
         """
         self._keep_alive()
@@ -104,32 +104,34 @@
             payload["title"] = title
             payload["prompt"] = prompt
         else:
             payload["gpt_description_prompt"] = prompt
 
         response = self.client.post(
             f"{Suno.BASE_URL}/api/generate/v2/", json=payload)
+        logger.info(response.text)
 
         if response.status_code != 200:
-            logger.info("Audio Generate Failed ⁉️")
+            logger.error("Audio Generate Failed ⁉️")
             raise Exception(f"Error response: {response.text}")
 
         song_ids = [audio['id'] for audio in response.json()['clips']]
         if wait_audio:
             return self._wait_for_audio(song_ids)
         else:
             self._keep_alive(True)
             logger.info("Generated Audio Successfully ✅")
             return response_to_clips(response.json()['clips'])
 
     def _wait_for_audio(self, song_ids):
         """Helper method to wait for audio processing to complete."""
         start_time = time.time()
         last_clips = []
-        while time.time() - start_time < 100:  # Timeout after 100 seconds
+        time.sleep(random.uniform(10, 20))  # Wait
+        while time.time() - start_time < 200:  # Timeout after 200 seconds
             clips = self.get_songs(song_ids)
             all_completed = all(
                 audio.status in ['streaming', 'complete'] for audio in clips)
             if all_completed:
                 logger.info("Generated Audio Successfully ✅")
                 return clips
             last_clips = clips
@@ -154,14 +156,15 @@
         """
         self._keep_alive()  # Ensure session is active
         url = f"{Suno.BASE_URL}/api/feed/"
         if song_ids:
             url += f"?ids={song_ids}"
         logger.info("Getting Songs Info...")
         response = self.client.get(url)  # Call API
+        logger.info(response.text)
         return response_to_clips(response.json())
 
     def get_song(self, id: str) -> Clip:
         """
         Retrieve a single song by its ID.
 
         Parameters:
@@ -170,22 +173,24 @@
         Returns:
         Clip: A Clip object containing details about the song, such as the audio URL, song status, and other metadata.
         """
         self._keep_alive()  # Ensure session is active
         logger.info("Getting Song Info...")
         response = self.client.get(
             f"{Suno.BASE_URL}/api/feed/?ids={id}")  # Call API
+        logger.info(response.text)
         return create_clip_from_data(response.json()[0])
 
     def get_credits(self) -> CreditsInfo:
         """Retrieve current billing and credits information."""
         self._keep_alive()  # Ensure session is active
         logger.info("Credits Info...")
         response = self.client.get(
             f"{Suno.BASE_URL}/api/billing/info/")  # Call API
+        logger.info(response.text)
         if response.status_code == 200:
             data = response.json()
             result = {
                 "credits_left": data["total_credits_left"],
                 "period": data["period"],
                 "monthly_limit": data["monthly_limit"],
                 "monthly_usage": data["monthly_usage"],
```

### Comparing `sunoai-1.0.1/suno/utils.py` & `sunoai-1.0.2/suno/utils.py`

 * *Files identical despite different names*

