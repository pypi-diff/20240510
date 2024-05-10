# Comparing `tmp/abstract_flask-0.0.0.6.tar.gz` & `tmp/abstract_flask-0.0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abstract_flask-0.0.0.6.tar", last modified: Fri May 10 08:20:32 2024, max compression
+gzip compressed data, was "abstract_flask-0.0.0.7.tar", last modified: Fri May 10 10:51:56 2024, max compression
```

## Comparing `abstract_flask-0.0.0.6.tar` & `abstract_flask-0.0.0.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-05-10 08:20:32.414655 abstract_flask-0.0.0.6/
--rw-r--r--   0 gamook    (1000) gamook    (1000)      572 2024-05-10 08:20:32.414655 abstract_flask-0.0.0.6/PKG-INFO
--rw-rw-r--   0 gamook    (1000) gamook    (1000)       49 2024-04-08 17:04:50.000000 abstract_flask-0.0.0.6/README.md
--rw-rw-r--   0 gamook    (1000) gamook    (1000)       38 2024-05-10 08:20:32.414655 abstract_flask-0.0.0.6/setup.cfg
--rw-rw-r--   0 gamook    (1000) gamook    (1000)      952 2024-05-10 08:20:27.000000 abstract_flask-0.0.0.6/setup.py
-drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-05-10 08:20:32.410655 abstract_flask-0.0.0.6/src/
-drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-05-10 08:20:32.414655 abstract_flask-0.0.0.6/src/abstract_flask/
--rw-rw-r--   0 gamook    (1000) gamook    (1000)       55 2024-05-10 05:52:34.000000 abstract_flask-0.0.0.6/src/abstract_flask/__init__.py
--rw-rw-r--   0 gamook    (1000) gamook    (1000)    12493 2024-05-10 08:20:20.000000 abstract_flask-0.0.0.6/src/abstract_flask/file_utils.py
--rw-rw-r--   0 gamook    (1000) gamook    (1000)      571 2024-05-10 01:11:01.000000 abstract_flask-0.0.0.6/src/abstract_flask/network_tools.py
-drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-05-10 08:20:32.414655 abstract_flask-0.0.0.6/src/abstract_flask.egg-info/
--rw-r--r--   0 gamook    (1000) gamook    (1000)      572 2024-05-10 08:20:32.000000 abstract_flask-0.0.0.6/src/abstract_flask.egg-info/PKG-INFO
--rw-rw-r--   0 gamook    (1000) gamook    (1000)      327 2024-05-10 08:20:32.000000 abstract_flask-0.0.0.6/src/abstract_flask.egg-info/SOURCES.txt
--rw-rw-r--   0 gamook    (1000) gamook    (1000)        1 2024-05-10 08:20:32.000000 abstract_flask-0.0.0.6/src/abstract_flask.egg-info/dependency_links.txt
--rw-rw-r--   0 gamook    (1000) gamook    (1000)       40 2024-05-10 08:20:32.000000 abstract_flask-0.0.0.6/src/abstract_flask.egg-info/requires.txt
--rw-rw-r--   0 gamook    (1000) gamook    (1000)       15 2024-05-10 08:20:32.000000 abstract_flask-0.0.0.6/src/abstract_flask.egg-info/top_level.txt
+drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-05-10 10:51:56.519057 abstract_flask-0.0.0.7/
+-rw-r--r--   0 gamook    (1000) gamook    (1000)      572 2024-05-10 10:51:56.519057 abstract_flask-0.0.0.7/PKG-INFO
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)       49 2024-04-08 17:04:50.000000 abstract_flask-0.0.0.7/README.md
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)       38 2024-05-10 10:51:56.519057 abstract_flask-0.0.0.7/setup.cfg
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)      952 2024-05-10 10:51:34.000000 abstract_flask-0.0.0.7/setup.py
+drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-05-10 10:51:56.519057 abstract_flask-0.0.0.7/src/
+drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-05-10 10:51:56.519057 abstract_flask-0.0.0.7/src/abstract_flask/
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)       55 2024-05-10 05:52:34.000000 abstract_flask-0.0.0.7/src/abstract_flask/__init__.py
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)    12389 2024-05-10 10:51:18.000000 abstract_flask-0.0.0.7/src/abstract_flask/file_utils.py
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)      571 2024-05-10 01:11:01.000000 abstract_flask-0.0.0.7/src/abstract_flask/network_tools.py
+drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-05-10 10:51:56.519057 abstract_flask-0.0.0.7/src/abstract_flask.egg-info/
+-rw-r--r--   0 gamook    (1000) gamook    (1000)      572 2024-05-10 10:51:56.000000 abstract_flask-0.0.0.7/src/abstract_flask.egg-info/PKG-INFO
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)      327 2024-05-10 10:51:56.000000 abstract_flask-0.0.0.7/src/abstract_flask.egg-info/SOURCES.txt
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)        1 2024-05-10 10:51:56.000000 abstract_flask-0.0.0.7/src/abstract_flask.egg-info/dependency_links.txt
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)       40 2024-05-10 10:51:56.000000 abstract_flask-0.0.0.7/src/abstract_flask.egg-info/requires.txt
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)       15 2024-05-10 10:51:56.000000 abstract_flask-0.0.0.7/src/abstract_flask.egg-info/top_level.txt
```

### Comparing `abstract_flask-0.0.0.6/PKG-INFO` & `abstract_flask-0.0.0.7/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abstract_flask
-Version: 0.0.0.6
+Version: 0.0.0.7
 Author: putkoff
 Author-email: partners@abstractendeavors.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `abstract_flask-0.0.0.6/setup.py` & `abstract_flask-0.0.0.7/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from time import time
 import setuptools
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 setuptools.setup(
     name='abstract_flask',
-    version='0.0.0.6',
+    version='0.0.0.7',
     author='putkoff',
     author_email='partners@abstractendeavors.com',
     description="",
     long_description=long_description,
     long_description_content_type='text/markdown',
     classifiers=[
           'Development Status :: 3 - Alpha',
```

### Comparing `abstract_flask-0.0.0.6/src/abstract_flask/file_utils.py` & `abstract_flask-0.0.0.7/src/abstract_flask/file_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,31 +67,31 @@
 
     def get_user_saved_dir(self, user):
         return self.make_user_dir(user, 'saved')
     # File path generation (without creating directories)
     def get_file_path(self, directory, fileName):
         return os.path.join(directory, fileName)
 def get_user_downloads_file_path(user,fileName):
-    abs_manager = AbsManager.get_instance()
+    abs_manager = AbsManager()
     user_downloads_dir = abs_manager.get_user_downloads_dir(user)
     return abs_manager.get_file_path(user_downloads_dir, fileName)
 def get_user_process_file_path(user,fileName):
-    abs_manager = AbsManager.get_instance()
+    abs_manager = AbsManager()
     user_process_dir = abs_manager.get_user_process_dir(user)
     return abs_manager.get_file_path(user_process_dir, fileName)
 def get_user_uploads_file_path(user,fileName):
-    abs_manager = AbsManager.get_instance()
+    abs_manager = AbsManager()
     user_uploads_dir = abs_manager.get_user_uploads_dir(user)
     return abs_manager.get_file_path(user_uploads_dir, fileName)
 def get_user_saved_file_path(user,fileName):
-    abs_manager = AbsManager.get_instance()
+    abs_manager = AbsManager()
     user_saved_dir = abs_manager.get_user_saved_dir(user)
     return abs_manager.get_file_path(user_saved_dir, fileName)
 def get_user_converts_file_path(user,fileName):
-    abs_manager = AbsManager.get_instance()
+    abs_manager = AbsManager()
     user_converts_dir = abs_manager.get_user_converts_dir(user)
     return abs_manager.get_file_path(user_converts_dir, fileName)
 def copy_to(path_1,path_2):
     if os.path.isfile(path_1):
         shutil.copy(path_1,path_2)
         print(f"copyd from {path_1}\n to {path_2}\n\n")
         return path_2
@@ -198,15 +198,15 @@
 def cleanup_files(*paths):
     """Remove files from the filesystem as a cleanup process."""
     for path in paths:
         if os.path.isfile(path):
             os.remove(path)
 
 def allowed_file(filename):
-    return '.' in filename and filename.rsplit('.', 1)[1].lower() in fileManager.get_instance().allowed_extentions
+    return '.' in filename and filename.rsplit('.', 1)[1].lower() in fileManager().allowed_extentions
 
 def read_file(file=None,file_path=None):
     if file and is_storage(file):
         return file.read()
     elif file_path and os.path.splitext(file_path)[-1][1:] in ['ods','csv','xls','xlsx','xlsb']:
          return get_df(file_path)
     else:
@@ -229,18 +229,18 @@
         return secure_filename(obj.filename)
     if isinstance(obj, str) and (os.path.isfile(obj) or os.path.isdir(os.path.dirname(obj))):
         return os.path.basename(obj)
     return str(obj)
 
 
 def get_path_from_result(user,fileName,success=True,directory=None):
-    abs_manager = AbsManager.get_instance()
+    abs_manager = AbsManager()
     return os.path.join(abs_manager.make_user_dir(user,directory),fileName)
 def save_to_directory(contents,user,fileName,success=True,directory=None):
-    abs_manager = AbsManager.get_instance()
+    abs_manager = AbsManager()
     if (directory != 'process' and success != 'override') or (abs_manager.check_user_dir(user,directory) == False and success != 'override'):
         return {'success': False, 'fileName': fileName, "user": user,"directory":directory}
     
     safe_excel_save(get_df(contents),os.path.join(abs_manager.make_user_dir(user,directory),fileName))
     return {'success': True, 'fileName': fileName, "user": user,"directory":directory}
 
 def upload_file(file, user=None):
```

### Comparing `abstract_flask-0.0.0.6/src/abstract_flask/network_tools.py` & `abstract_flask-0.0.0.7/src/abstract_flask/network_tools.py`

 * *Files identical despite different names*

### Comparing `abstract_flask-0.0.0.6/src/abstract_flask.egg-info/PKG-INFO` & `abstract_flask-0.0.0.7/src/abstract_flask.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abstract_flask
-Version: 0.0.0.6
+Version: 0.0.0.7
 Author: putkoff
 Author-email: partners@abstractendeavors.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```

