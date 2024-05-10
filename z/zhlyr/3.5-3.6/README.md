# Comparing `tmp/zhlyr-3.5.tar.gz` & `tmp/zhlyr-3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zhlyr-3.5.tar", last modified: Fri May 10 14:03:29 2024, max compression
+gzip compressed data, was "zhlyr-3.6.tar", last modified: Fri May 10 18:23:20 2024, max compression
```

## Comparing `zhlyr-3.5.tar` & `zhlyr-3.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-10 14:03:29.820569 zhlyr-3.5/
--rw-rw-rw-   0        0        0      889 2024-05-10 14:03:29.818568 zhlyr-3.5/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-05-10 14:03:29.820569 zhlyr-3.5/setup.cfg
--rw-rw-rw-   0        0        0     1079 2024-05-10 14:02:21.000000 zhlyr-3.5/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-10 14:03:29.801944 zhlyr-3.5/zhlyr/
--rw-rw-rw-   0        0        0       92 2024-05-10 14:01:33.000000 zhlyr-3.5/zhlyr/__init__.py
--rw-rw-rw-   0        0        0     1445 2024-05-10 10:49:35.000000 zhlyr-3.5/zhlyr/recosnize.py
--rw-rw-rw-   0        0        0     1933 2024-05-10 13:40:19.000000 zhlyr-3.5/zhlyr/serilize.py
--rw-rw-rw-   0        0        0     2159 2024-05-10 13:04:05.000000 zhlyr-3.5/zhlyr/zhlyr.py
-drwxrwxrwx   0        0        0        0 2024-05-10 14:03:29.816560 zhlyr-3.5/zhlyr.egg-info/
--rw-rw-rw-   0        0        0      889 2024-05-10 14:03:29.000000 zhlyr-3.5/zhlyr.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      194 2024-05-10 14:03:29.000000 zhlyr-3.5/zhlyr.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-10 14:03:29.000000 zhlyr-3.5/zhlyr.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2024-05-10 14:03:29.000000 zhlyr-3.5/zhlyr.egg-info/top_level.txt
+drwxrwxrwx   0 whoami    (1000) whoami    (1000)        0 2024-05-10 18:23:20.100962 zhlyr-3.6/
+-rwxrwxrwx   0 whoami    (1000) whoami    (1000)      865 2024-05-10 18:23:20.094958 zhlyr-3.6/PKG-INFO
+-rwxrwxrwx   0 whoami    (1000) whoami    (1000)       38 2024-05-10 18:23:20.101966 zhlyr-3.6/setup.cfg
+-rwxrwxrwx   0 whoami    (1000) whoami    (1000)     1081 2024-05-10 18:21:36.000000 zhlyr-3.6/setup.py
+drwxrwxrwx   0 whoami    (1000) whoami    (1000)        0 2024-05-10 18:23:20.021823 zhlyr-3.6/zhlyr/
+-rwxrwxrwx   0 whoami    (1000) whoami    (1000)       92 2024-05-10 14:01:33.000000 zhlyr-3.6/zhlyr/__init__.py
+-rwxrwxrwx   0 whoami    (1000) whoami    (1000)     1445 2024-05-10 10:49:35.000000 zhlyr-3.6/zhlyr/recosnize.py
+-rwxrwxrwx   0 whoami    (1000) whoami    (1000)     1933 2024-05-10 13:40:19.000000 zhlyr-3.6/zhlyr/serilize.py
+-rwxrwxrwx   0 whoami    (1000) whoami    (1000)     2159 2024-05-10 13:04:05.000000 zhlyr-3.6/zhlyr/zhlyr.py
+drwxrwxrwx   0 whoami    (1000) whoami    (1000)        0 2024-05-10 18:23:20.088322 zhlyr-3.6/zhlyr.egg-info/
+-rwxrwxrwx   0 whoami    (1000) whoami    (1000)      865 2024-05-10 18:23:19.000000 zhlyr-3.6/zhlyr.egg-info/PKG-INFO
+-rwxrwxrwx   0 whoami    (1000) whoami    (1000)      194 2024-05-10 18:23:19.000000 zhlyr-3.6/zhlyr.egg-info/SOURCES.txt
+-rwxrwxrwx   0 whoami    (1000) whoami    (1000)        1 2024-05-10 18:23:19.000000 zhlyr-3.6/zhlyr.egg-info/dependency_links.txt
+-rwxrwxrwx   0 whoami    (1000) whoami    (1000)        6 2024-05-10 18:23:19.000000 zhlyr-3.6/zhlyr.egg-info/top_level.txt
```

### Comparing `zhlyr-3.5/PKG-INFO` & `zhlyr-3.6/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-Metadata-Version: 2.1
-Name: zhlyr
-Version: 3.5
-Summary: Python library for music handling
-Home-page: https://github.com/Gaoc3/zhlyr
-Author: Mtsky
-Author-email: secon2636@gmail.com
-License: MIT
-Keywords: lyrics,music,shazam,serialize,serializer,recognize
-Classifier: Development Status :: 1 - Planning
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: Unix
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: Microsoft :: Windows
-Requires: requests
-Requires: shazamio
-Requires: shazam
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-
-**A python package to get lyrics from music , serialize data from json response and recognize data from musics**
+Metadata-Version: 2.1
+Name: zhlyr
+Version: 3.6
+Summary: Python library for music handling
+Home-page: https://github.com/Gaoc3/zhlyr
+Author: Mtsky
+Author-email: secon2636@gmail.com
+License: MIT
+Keywords: lyrics,music,shazam,serialize,serializer,recognize
+Classifier: Development Status :: 1 - Planning
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: Unix
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Operating System :: Microsoft :: Windows
+Requires: requests
+Requires: shazamio
+Requires: shazam
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+
+**A python package to get lyrics from music , serialize data from json response and recognize data from musics**
```

### Comparing `zhlyr-3.5/setup.py` & `zhlyr-3.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup , find_packages
 
 setup(
     name = 'zhlyr',
-    version = '3.5',
+    version = '3.6',
     packages = find_packages(),
     requires = ['requests','shazamio','shazam'],
     long_description ='**A python package to get lyrics from music , serialize data from json response and recognize data from musics**',
     long_description_content_type='text/markdown',
     description = 'Python library for music handling',
     author = 'Mtsky',
     author_email = 'secon2636@gmail.com',
@@ -20,8 +20,8 @@
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: Microsoft :: Windows",
     ],
     keywords= ['lyrics','music','shazam','serialize','serializer','recognize'],
     python_requires=">=3.9"
-)
+)
```

### Comparing `zhlyr-3.5/zhlyr/recosnize.py` & `zhlyr-3.6/zhlyr/recosnize.py`

 * *Files identical despite different names*

### Comparing `zhlyr-3.5/zhlyr/serilize.py` & `zhlyr-3.6/zhlyr/serilize.py`

 * *Files identical despite different names*

### Comparing `zhlyr-3.5/zhlyr/zhlyr.py` & `zhlyr-3.6/zhlyr/zhlyr.py`

 * *Files identical despite different names*

### Comparing `zhlyr-3.5/zhlyr.egg-info/PKG-INFO` & `zhlyr-3.6/zhlyr.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-Metadata-Version: 2.1
-Name: zhlyr
-Version: 3.5
-Summary: Python library for music handling
-Home-page: https://github.com/Gaoc3/zhlyr
-Author: Mtsky
-Author-email: secon2636@gmail.com
-License: MIT
-Keywords: lyrics,music,shazam,serialize,serializer,recognize
-Classifier: Development Status :: 1 - Planning
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: Unix
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: Microsoft :: Windows
-Requires: requests
-Requires: shazamio
-Requires: shazam
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-
-**A python package to get lyrics from music , serialize data from json response and recognize data from musics**
+Metadata-Version: 2.1
+Name: zhlyr
+Version: 3.6
+Summary: Python library for music handling
+Home-page: https://github.com/Gaoc3/zhlyr
+Author: Mtsky
+Author-email: secon2636@gmail.com
+License: MIT
+Keywords: lyrics,music,shazam,serialize,serializer,recognize
+Classifier: Development Status :: 1 - Planning
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: Unix
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Operating System :: Microsoft :: Windows
+Requires: requests
+Requires: shazamio
+Requires: shazam
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+
+**A python package to get lyrics from music , serialize data from json response and recognize data from musics**
```

