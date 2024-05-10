# Comparing `tmp/abstract_flask-0.0.0.3.tar.gz` & `tmp/abstract_flask-0.0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abstract_flask-0.0.0.3.tar", last modified: Fri May 10 05:59:56 2024, max compression
+gzip compressed data, was "abstract_flask-0.0.0.4.tar", last modified: Fri May 10 07:29:14 2024, max compression
```

## Comparing `abstract_flask-0.0.0.3.tar` & `abstract_flask-0.0.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-05-10 05:59:56.983228 abstract_flask-0.0.0.3/
--rw-r--r--   0 gamook    (1000) gamook    (1000)      572 2024-05-10 05:59:56.983228 abstract_flask-0.0.0.3/PKG-INFO
--rw-rw-r--   0 gamook    (1000) gamook    (1000)       49 2024-04-08 17:04:50.000000 abstract_flask-0.0.0.3/README.md
--rw-rw-r--   0 gamook    (1000) gamook    (1000)       38 2024-05-10 05:59:56.983228 abstract_flask-0.0.0.3/setup.cfg
--rw-rw-r--   0 gamook    (1000) gamook    (1000)      952 2024-05-10 05:59:44.000000 abstract_flask-0.0.0.3/setup.py
-drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-05-10 05:59:56.983228 abstract_flask-0.0.0.3/src/
-drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-05-10 05:59:56.983228 abstract_flask-0.0.0.3/src/abstract_flask/
--rw-rw-r--   0 gamook    (1000) gamook    (1000)       55 2024-05-10 05:52:34.000000 abstract_flask-0.0.0.3/src/abstract_flask/__init__.py
--rw-rw-r--   0 gamook    (1000) gamook    (1000)    11224 2024-05-10 05:59:28.000000 abstract_flask-0.0.0.3/src/abstract_flask/file_utils.py
--rw-rw-r--   0 gamook    (1000) gamook    (1000)      571 2024-05-10 01:11:01.000000 abstract_flask-0.0.0.3/src/abstract_flask/network_tools.py
-drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-05-10 05:59:56.983228 abstract_flask-0.0.0.3/src/abstract_flask.egg-info/
--rw-r--r--   0 gamook    (1000) gamook    (1000)      572 2024-05-10 05:59:56.000000 abstract_flask-0.0.0.3/src/abstract_flask.egg-info/PKG-INFO
--rw-rw-r--   0 gamook    (1000) gamook    (1000)      327 2024-05-10 05:59:56.000000 abstract_flask-0.0.0.3/src/abstract_flask.egg-info/SOURCES.txt
--rw-rw-r--   0 gamook    (1000) gamook    (1000)        1 2024-05-10 05:59:56.000000 abstract_flask-0.0.0.3/src/abstract_flask.egg-info/dependency_links.txt
--rw-rw-r--   0 gamook    (1000) gamook    (1000)       40 2024-05-10 05:59:56.000000 abstract_flask-0.0.0.3/src/abstract_flask.egg-info/requires.txt
--rw-rw-r--   0 gamook    (1000) gamook    (1000)       15 2024-05-10 05:59:56.000000 abstract_flask-0.0.0.3/src/abstract_flask.egg-info/top_level.txt
+drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-05-10 07:29:14.357315 abstract_flask-0.0.0.4/
+-rw-r--r--   0 gamook    (1000) gamook    (1000)      572 2024-05-10 07:29:14.357315 abstract_flask-0.0.0.4/PKG-INFO
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)       49 2024-04-08 17:04:50.000000 abstract_flask-0.0.0.4/README.md
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)       38 2024-05-10 07:29:14.357315 abstract_flask-0.0.0.4/setup.cfg
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)      952 2024-05-10 07:29:08.000000 abstract_flask-0.0.0.4/setup.py
+drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-05-10 07:29:14.357315 abstract_flask-0.0.0.4/src/
+drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-05-10 07:29:14.357315 abstract_flask-0.0.0.4/src/abstract_flask/
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)       55 2024-05-10 05:52:34.000000 abstract_flask-0.0.0.4/src/abstract_flask/__init__.py
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)    12916 2024-05-10 07:28:48.000000 abstract_flask-0.0.0.4/src/abstract_flask/file_utils.py
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)      571 2024-05-10 01:11:01.000000 abstract_flask-0.0.0.4/src/abstract_flask/network_tools.py
+drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-05-10 07:29:14.357315 abstract_flask-0.0.0.4/src/abstract_flask.egg-info/
+-rw-r--r--   0 gamook    (1000) gamook    (1000)      572 2024-05-10 07:29:14.000000 abstract_flask-0.0.0.4/src/abstract_flask.egg-info/PKG-INFO
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)      327 2024-05-10 07:29:14.000000 abstract_flask-0.0.0.4/src/abstract_flask.egg-info/SOURCES.txt
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)        1 2024-05-10 07:29:14.000000 abstract_flask-0.0.0.4/src/abstract_flask.egg-info/dependency_links.txt
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)       40 2024-05-10 07:29:14.000000 abstract_flask-0.0.0.4/src/abstract_flask.egg-info/requires.txt
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)       15 2024-05-10 07:29:14.000000 abstract_flask-0.0.0.4/src/abstract_flask.egg-info/top_level.txt
```

### Comparing `abstract_flask-0.0.0.3/PKG-INFO` & `abstract_flask-0.0.0.4/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abstract_flask
-Version: 0.0.0.3
+Version: 0.0.0.4
 Author: putkoff
 Author-email: partners@abstractendeavors.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `abstract_flask-0.0.0.3/setup.py` & `abstract_flask-0.0.0.4/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from time import time
 import setuptools
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 setuptools.setup(
     name='abstract_flask',
-    version='0.0.0.3',
+    version='0.0.0.4',
     author='putkoff',
     author_email='partners@abstractendeavors.com',
     description="",
     long_description=long_description,
     long_description_content_type='text/markdown',
     classifiers=[
           'Development Status :: 3 - Alpha',
```

### Comparing `abstract_flask-0.0.0.3/src/abstract_flask/file_utils.py` & `abstract_flask-0.0.0.4/src/abstract_flask/file_utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os,time,random,hashlib,shutil
 from flask import jsonify
 from werkzeug.utils import secure_filename
-from abstract_pandas import get_df,safe_excel_save
+from abstract_pandas import get_df,safe_excel_save,is_file
 from werkzeug.datastructures import FileStorage
 import os
 class fileManager:
     _instance = None
 
     def __init__(self, allowed_extentions=None):
         if fileManager._instance is not None:
@@ -57,34 +57,41 @@
         return self._make_dir(os.path.join(self.get_base_path(), 'users'))
 
     def get_uploads_dir(self):
         return self._make_dir(os.path.join(self.get_base_path(), 'uploads'))
 
     def get_downloads_dir(self):
         return self._make_dir(os.path.join(self.get_base_path(), 'downloads'))
-
-    # User-specific directories
-    def get_user_dir(self, user):
-        return self._make_dir(os.path.join(self.get_users_dir(), user))
     
+    # User-specific directories
+    def get_user_dir(self, user,sub_path=None):
+        user_path = os.path.join(self.get_users_dir(), user)
+        if sub_path:
+            user_path = os.path.join(user_path,sub_path)
+        return user_path
+    def check_user_dir(self,user,sub_path=None):
+        user_file_dir = self.get_user_dir(user,sub_path=sub_path)
+        return os.path.isdir(user_file_dir)
+    def make_user_dir(self,user,sub_path=None):
+        self._make_dir(self.get_user_dir(user))
+        return self._make_dir(self.get_user_dir(user,sub_path))
     def get_user_converts_dir(self, user):
-        return self._make_dir(os.path.join(self.get_user_dir(user), 'converts'))
+        return self.make_user_dir(user, 'converts')
 
     def get_user_uploads_dir(self, user):
-        return self._make_dir(os.path.join(self.get_user_dir(user), 'uploads'))
+        return self.make_user_dir(user, 'uploads')
 
     def get_user_downloads_dir(self, user):
-        return self._make_dir(os.path.join(self.get_user_dir(user), 'downloads'))
+        return self.make_user_dir(user,  'downloads')
 
     def get_user_process_dir(self, user):
-        return self._make_dir(os.path.join(self.get_user_dir(user), 'process'))
+        return self.make_user_dir(user,'process')
 
     def get_user_saved_dir(self, user):
-        return self._make_dir(os.path.join(self.get_user_dir(user), 'saved'))
-
+        return self.make_user_dir(user, 'saved')
     # File path generation (without creating directories)
     def get_file_path(self, directory, fileName):
         return os.path.join(directory, fileName)
 def get_user_downloads_file_path(user,fileName):
     abs_manager = AbsManager.get_instance()
     user_downloads_dir = abs_manager.get_user_downloads_dir(user)
     return abs_manager.get_file_path(user_downloads_dir, fileName)
@@ -126,59 +133,61 @@
             shutil.move(path_1,path_2)
         except:
             return manual_move(path_1,path_2)
         print(f"moved from {path_1} to {path_2}\n\n")
         return path_2
     print(f"not moved from {path_1} to {path_2}\n\n")
     return False
-def move_from_process(user,fileName):
+def move_to_download(user,fileName,success=True,directory=None):
     process_file_path = get_user_process_file_path(user,fileName)
     downloads_file_path = get_user_downloads_file_path(user,fileName)
-    return move_to(process_file_path,downloads_file_path)
-def move_to_process(user,fileName):
+    if move_to(process_file_path,downloads_file_path) == False:
+        return {'success': False, 'fileName': fileName, "user": user,"directory":"process"}
+    return {'success': True, 'fileName': fileName, "user": user,"directory":"downloads"}
+def move_to_process(user,fileName,success=True,directory=None):
     uploads_file_path = get_user_uploads_file_path(user,fileName)
     process_file_path = get_user_process_file_path(user,fileName)
-    return move_to(uploads_file_path,process_file_path)
-def copy_to_saved(user,fileName):
+    if move_to(uploads_file_path,process_file_path) == False:
+        return {'success': False, 'fileName': fileName, "user": user,"directory":"uploads"}
+    return {'success': True, 'fileName': fileName, "user": user,"directory":"process"}
+def copy_to_saved(user,fileName,success=True,directory=None):
     downloads_file_path = get_user_downloads_file_path(user,fileName)
     saved_file_path = get_user_saved_file_path(user,fileName)
-    return copy_to(downloads_file_path,saved_file_path)
+    if copy_to(downloads_file_path,saved_file_path) == False:
+        return {'success': False, 'fileName': fileName, "user": user,"directory":"downloads"}
+    return {'success': True, 'fileName': fileName, "user": user,"directory":"saved"}
 def convert_file(file_path,converts_file_path):
     original_dirName = get_dirname(file_path)
     conv_file_name = get_file_name(converts_file_path)
     new_file_path = os.path.join(original_dirName,conv_file_name)
     moved = move_to(converts_file_path,new_file_path)
     if moved:
         cleanup_files(file_path)
         return moved
     return False
 def is_storage(obj):
-    if isinstance(obj, FileStorage):  # Check if source is a FileStorage object
-        return True
-    return False
+    """Check if an object is of type FileStorage."""
+    return isinstance(obj, FileStorage)
 def get_file_name(obj):
     if is_storage(obj):
         try:
             # Read the file directly from the file object
             file_name = secure_filename(obj.filename)
             return file_name
         except Exception as e:
             print(f"Failed to read file: {e}")
     if isinstance(obj,str) and (os.path.isfile(obj) or os.path.isdir(os.path.dirname(obj))):
          return os.path.basename(obj)
     return obj
 def generate_custom_uid():
-    """
-    Generates a custom unique identifier using a combination of the current time (to the millisecond)
-    and a random number, hashed for uniformity and to obscure the raw data.
-    """
+    """Generate a custom unique identifier."""
     timestamp = int(time.time() * 1000)  # Current time in milliseconds
     random_int = random.randint(0, 999999)  # Random integer
     raw_uid = f"{timestamp}-{random_int}"
-    hash_uid = hashlib.sha256(raw_uid.encode()).hexdigest()  # Creating a SHA-256 hash of the ID
+    hash_uid = hashlib.sha256(raw_uid.encode()).hexdigest()
     return hash_uid[:16]  # Return the first 16 characters for a shorter UID
 def insert_into_tail(file_path,string):
     dirName = os.path.dirname(file_path)
     baseName = os.path.basename(file_path)
     fileName,ext=os.path.splitext(baseName)
     newName = f"{fileName}_{string}{ext}"
     if dirName:
@@ -186,14 +195,15 @@
     return newName
 def get_unique_file_name(obj):
     dirname = get_dirname(obj)
     fileName= insert_into_tail(get_file_name(obj),generate_custom_uid())
     if dirname:
         return os.path.join(dirname,fileName)
     return fileName
+
 def validate_user_and_filename(user, filename):
     """Validate presence of user and filename."""
     if not user or not filename:
         return jsonify({'error': True, 'message': "User or filename not specified"}), 400
     return None
 
 def file_exists(file_path):
@@ -231,39 +241,57 @@
          safe_excel_save(get_df(file_path),file_path)
     else:
         write_to_file(contents=file,file_path=file_path)
 def get_dirname(obj):
     if isinstance(obj,str) and (os.path.isfile(obj) or os.path.isdir(os.path.dirname(obj))):
         return os.path.dirname(obj)
 def get_file_name(obj):
+    """Get a safe filename from a file or string path."""
     if is_storage(obj):
-        try:
-            # Read the file directly from the file object
-            filename = secure_filename(obj.filename)
-            return filename
-        except Exception as e:
-            print(f"Failed to read file: {e}")
-    if isinstance(obj,str) and (os.path.isfile(obj) or os.path.isdir(os.path.dirname(obj))):
-         return os.path.basename(obj)
-    return obj
+        return secure_filename(obj.filename)
+    if isinstance(obj, str) and (os.path.isfile(obj) or os.path.isdir(os.path.dirname(obj))):
+        return os.path.basename(obj)
+    return str(obj)
+
 
-def upload_file(file,user=None):
-    if not file:
+def get_path_from_result(user,fileName,success=True,directory=None):
+    abs_manager = AbsManager.get_instance()
+    return os.path.join(abs_manager.make_user_dir(user,directory),fileName)
+def save_to_directory(contents,user,fileName,success=True,directory=None):
+    abs_manager = AbsManager.get_instance()
+    if (directory != 'process' and success != 'override') or (abs_manager.check_user_dir(user,directory) == False and success != 'override'):
+        return {'success': False, 'fileName': fileName, "user": user,"directory":directory}
+    
+    safe_excel_save(get_df(contents),os.path.join(abs_manager.make_user_dir(user,directory),fileName))
+    return {'success': True, 'fileName': fileName, "user": user,"directory":directory}
+
+def upload_file(file, user=None):
+    """Main file upload function to handle different types of files."""
+    if file is None:
         return jsonify({'error': True, 'message': "No file uploaded"}), 400
+    
+        
+    # Determine a safe filename
     filename = get_file_name(file)
     if not allowed_file(filename):
         return jsonify({'error': True, 'message': "File type not allowed"}), 400
     
-    if user == None:
-        user='Defaut'
+    # Set a default user if not specified
+    user = user or 'Default'
+    
+    # Generate a unique file name and the upload path
     unique_name = get_unique_file_name(filename)
-    upload_file_path = get_user_uploads_file_path(user,unique_name)
-    save_file(file,upload_file_path)
-    return {'success': True, 'fileName': unique_name,"user":user}
+    upload_file_path = get_user_uploads_file_path(user, unique_name)
+    if is_file(file):
+        copy_to(file,upload_file_path)
+    else:
+        # Save the file at the specified path
+        save_file(file, upload_file_path)
 
+    return {'success': True, 'fileName': unique_name, "user": user,"directory":"upload"}
 def download_user_file(user=None,fileName=None):
     upload_file_path = get_user_uploads_file_path(user, fileName)
     download_file_path = get_user_downloads_file_path(user, fileName)
     processed_file_path = get_user_process_file_path(user, fileName)
     upload_file_veri = os.path.isfile(upload_file_path)
     processed_file_veri = os.path.isfile(processed_file_path)
     download_file_veri = os.path.isfile(download_file_path)
```

### Comparing `abstract_flask-0.0.0.3/src/abstract_flask/network_tools.py` & `abstract_flask-0.0.0.4/src/abstract_flask/network_tools.py`

 * *Files identical despite different names*

### Comparing `abstract_flask-0.0.0.3/src/abstract_flask.egg-info/PKG-INFO` & `abstract_flask-0.0.0.4/src/abstract_flask.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abstract_flask
-Version: 0.0.0.3
+Version: 0.0.0.4
 Author: putkoff
 Author-email: partners@abstractendeavors.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```

