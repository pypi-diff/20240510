# Comparing `tmp/VisioNomicon-0.1.1.tar.gz` & `tmp/VisioNomicon-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "VisioNomicon-0.1.1.tar", last modified: Tue Jan  2 20:36:47 2024, max compression
+gzip compressed data, was "VisioNomicon-0.1.2.tar", last modified: Fri Jan  5 23:55:56 2024, max compression
```

## Comparing `VisioNomicon-0.1.1.tar` & `VisioNomicon-0.1.2.tar`

### file list

```diff
@@ -1,18 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-02 20:36:47.129021 VisioNomicon-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-01-02 20:36:38.000000 VisioNomicon-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5538 2024-01-02 20:36:47.129021 VisioNomicon-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4825 2024-01-02 20:36:38.000000 VisioNomicon-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-02 20:36:47.129021 VisioNomicon-0.1.1/VisioNomicon/
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-01-02 20:36:38.000000 VisioNomicon-0.1.1/VisioNomicon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4755 2024-01-02 20:36:38.000000 VisioNomicon-0.1.1/VisioNomicon/args_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     3804 2024-01-02 20:36:38.000000 VisioNomicon-0.1.1/VisioNomicon/gpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     4169 2024-01-02 20:36:38.000000 VisioNomicon-0.1.1/VisioNomicon/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-02 20:36:47.129021 VisioNomicon-0.1.1/VisioNomicon.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5538 2024-01-02 20:36:47.000000 VisioNomicon-0.1.1/VisioNomicon.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-01-02 20:36:47.000000 VisioNomicon-0.1.1/VisioNomicon.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-02 20:36:47.000000 VisioNomicon-0.1.1/VisioNomicon.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-01-02 20:36:47.000000 VisioNomicon-0.1.1/VisioNomicon.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-01-02 20:36:47.000000 VisioNomicon-0.1.1/VisioNomicon.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-01-02 20:36:47.000000 VisioNomicon-0.1.1/VisioNomicon.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-02 20:36:47.133021 VisioNomicon-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-01-02 20:36:38.000000 VisioNomicon-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 23:55:56.256975 VisioNomicon-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-01-05 23:55:48.000000 VisioNomicon-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5538 2024-01-05 23:55:56.256975 VisioNomicon-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4825 2024-01-05 23:55:48.000000 VisioNomicon-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 23:55:56.256975 VisioNomicon-0.1.2/VisioNomicon/
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-01-05 23:55:48.000000 VisioNomicon-0.1.2/VisioNomicon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4755 2024-01-05 23:55:48.000000 VisioNomicon-0.1.2/VisioNomicon/args_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3804 2024-01-05 23:55:48.000000 VisioNomicon-0.1.2/VisioNomicon/gpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4209 2024-01-05 23:55:48.000000 VisioNomicon-0.1.2/VisioNomicon/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 23:55:56.256975 VisioNomicon-0.1.2/VisioNomicon.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5538 2024-01-05 23:55:56.000000 VisioNomicon-0.1.2/VisioNomicon.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-01-05 23:55:56.000000 VisioNomicon-0.1.2/VisioNomicon.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-05 23:55:56.000000 VisioNomicon-0.1.2/VisioNomicon.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-01-05 23:55:56.000000 VisioNomicon-0.1.2/VisioNomicon.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-01-05 23:55:56.000000 VisioNomicon-0.1.2/VisioNomicon.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-01-05 23:55:56.000000 VisioNomicon-0.1.2/VisioNomicon.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-05 23:55:56.256975 VisioNomicon-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-01-05 23:55:48.000000 VisioNomicon-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 23:55:56.256975 VisioNomicon-0.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-01-05 23:55:48.000000 VisioNomicon-0.1.2/tests/test_mapping.py
```

### Comparing `VisioNomicon-0.1.1/LICENSE` & `VisioNomicon-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `VisioNomicon-0.1.1/PKG-INFO` & `VisioNomicon-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: VisioNomicon
-Version: 0.1.1
+Version: 0.1.2
 Summary: A utility leveraging GPT-4V for image file renaming based on content.
 Home-page: https://github.com/rehanzo/visionomicon
 Author: Rehan Rana
 Author-email: visionomicon@rehanzo.com
 Keywords: gpt-4 gpt-4v openai renaming images
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `VisioNomicon-0.1.1/README.md` & `VisioNomicon-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `VisioNomicon-0.1.1/VisioNomicon/args_handler.py` & `VisioNomicon-0.1.2/VisioNomicon/args_handler.py`

 * *Files identical despite different names*

### Comparing `VisioNomicon-0.1.1/VisioNomicon/gpt.py` & `VisioNomicon-0.1.2/VisioNomicon/gpt.py`

 * *Files identical despite different names*

### Comparing `VisioNomicon-0.1.1/VisioNomicon/main.py` & `VisioNomicon-0.1.2/VisioNomicon/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,34 +19,34 @@
   if args.files is not None:
     new_filepaths: list[str] = generate_mapping(args)
 
     # have new and old, put them together into a json and save
     save_mapping(args, new_filepaths)
 
   # if executing or undoing
-  if args.undo is not None or args.execute is not None:
-    arg = args.execute if args.execute is not None else args.undo
-    mapping_fp = get_mapping_name(arg)
-
-    og_filepaths: list[str] = []
-    new_filepaths: list[str] = []
-
-    with open(mapping_fp) as f:
-      data = json.load(f)
-      og_filepaths += list(data.keys())
-      new_filepaths += list(data.values())
-
-    from_fps = og_filepaths if args.execute is not None else new_filepaths
-    to_fps = new_filepaths if args.execute is not None else og_filepaths
-      
-    for i in range(len(from_fps)):
-      _, filename = os.path.split(to_fps[i])
-      print("Renaming {} to {}".format(from_fps[i], '.../' + filename))
-      os.rename(from_fps[i], to_fps[i])
-    
+  if args.undo or args.execute:
+    rel_mapping_fp = args.execute if args.execute else args.undo
+    rename_from_mapping(rel_mapping_fp, args.undo is not None)
+
+def rename_from_mapping(rel_mapping_fp: str, undo: bool = False):
+  mapping_fp = get_mapping_name(rel_mapping_fp)
+  og_filepaths: list[str] = []
+  new_filepaths: list[str] = []
+
+  with open(mapping_fp) as f:
+    data = json.load(f)
+    og_filepaths += list(data.keys())
+    new_filepaths += list(data.values())
+
+  from_fps, to_fps = (new_filepaths, og_filepaths) if undo else (og_filepaths, new_filepaths)
+  
+  for i in range(len(from_fps)):
+    _, filename = os.path.split(to_fps[i])
+    print("Renaming {} to {}".format(from_fps[i], '.../' + filename))
+    os.rename(from_fps[i], to_fps[i])
 
 def get_mapping_name(cli_fp: str):
   if cli_fp != NO_VAL:
     return cli_fp
   else:
     # Join the directory with the file pattern
     file_pattern = os.path.join(DATA_DIR, '*.json')
@@ -64,15 +64,15 @@
   # data ready to dump, need to get mapping filename
   mapping_filename = generate_mapping_name(args)
 
   with open(mapping_filename, 'w') as file:
     json.dump(data, file, indent=4)
 
 def generate_mapping_name(args) -> str:
-  return args.output if args.output else DATA_DIR + datetime.now().strftime("mapping-%Y-%m-%d-%H-%M-%S.json")
+  return args.output if args.output != NO_VAL else DATA_DIR + datetime.now().strftime("mapping-%Y-%m-%d-%H-%M-%S.json")
   
 def generate_mapping(args) -> list[str]:
   og_filepaths: list[str] = args.files
   new_filepaths: list[str] = copy.deepcopy(og_filepaths)
 
   for i in range(len(new_filepaths)):
     slicepoint = new_filepaths[i].rindex("/") + 1
```

### Comparing `VisioNomicon-0.1.1/VisioNomicon.egg-info/PKG-INFO` & `VisioNomicon-0.1.2/VisioNomicon.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: VisioNomicon
-Version: 0.1.1
+Version: 0.1.2
 Summary: A utility leveraging GPT-4V for image file renaming based on content.
 Home-page: https://github.com/rehanzo/visionomicon
 Author: Rehan Rana
 Author-email: visionomicon@rehanzo.com
 Keywords: gpt-4 gpt-4v openai renaming images
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `VisioNomicon-0.1.1/setup.py` & `VisioNomicon-0.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='VisioNomicon',
-    version='0.1.1',
+    version='0.1.2',
     author='Rehan Rana',
     author_email='visionomicon@rehanzo.com',
     description='A utility leveraging GPT-4V for image file renaming based on content.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/rehanzo/visionomicon',
     packages=find_packages(),
```

