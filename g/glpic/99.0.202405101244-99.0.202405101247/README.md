# Comparing `tmp/glpic-99.0.202405101244.tar.gz` & `tmp/glpic-99.0.202405101247.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glpic-99.0.202405101244.tar", last modified: Fri May 10 12:44:29 2024, max compression
+gzip compressed data, was "glpic-99.0.202405101247.tar", last modified: Fri May 10 12:47:30 2024, max compression
```

## Comparing `glpic-99.0.202405101244.tar` & `glpic-99.0.202405101247.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:44:29.128689 glpic-99.0.202405101244/
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-10 12:44:29.124689 glpic-99.0.202405101244/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-05-10 12:44:12.000000 glpic-99.0.202405101244/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:44:29.124689 glpic-99.0.202405101244/glpic/
--rw-r--r--   0 runner    (1001) docker     (127)    10051 2024-05-10 12:44:12.000000 glpic-99.0.202405101244/glpic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11655 2024-05-10 12:44:12.000000 glpic-99.0.202405101244/glpic/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:44:29.124689 glpic-99.0.202405101244/glpic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-10 12:44:29.000000 glpic-99.0.202405101244/glpic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-10 12:44:29.000000 glpic-99.0.202405101244/glpic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 12:44:29.000000 glpic-99.0.202405101244/glpic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-10 12:44:29.000000 glpic-99.0.202405101244/glpic.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 12:44:29.000000 glpic-99.0.202405101244/glpic.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-10 12:44:29.000000 glpic-99.0.202405101244/glpic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-10 12:44:29.000000 glpic-99.0.202405101244/glpic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 12:44:29.128689 glpic-99.0.202405101244/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      705 2024-05-10 12:44:28.000000 glpic-99.0.202405101244/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:47:30.089373 glpic-99.0.202405101247/
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-10 12:47:30.089373 glpic-99.0.202405101247/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-05-10 12:47:04.000000 glpic-99.0.202405101247/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:47:30.089373 glpic-99.0.202405101247/glpic/
+-rw-r--r--   0 runner    (1001) docker     (127)    10051 2024-05-10 12:47:04.000000 glpic-99.0.202405101247/glpic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11777 2024-05-10 12:47:04.000000 glpic-99.0.202405101247/glpic/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:47:30.089373 glpic-99.0.202405101247/glpic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-10 12:47:30.000000 glpic-99.0.202405101247/glpic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-10 12:47:30.000000 glpic-99.0.202405101247/glpic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 12:47:30.000000 glpic-99.0.202405101247/glpic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-10 12:47:30.000000 glpic-99.0.202405101247/glpic.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 12:47:30.000000 glpic-99.0.202405101247/glpic.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-10 12:47:30.000000 glpic-99.0.202405101247/glpic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-10 12:47:30.000000 glpic-99.0.202405101247/glpic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 12:47:30.089373 glpic-99.0.202405101247/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      705 2024-05-10 12:47:29.000000 glpic-99.0.202405101247/setup.py
```

### Comparing `glpic-99.0.202405101244/README.md` & `glpic-99.0.202405101247/README.md`

 * *Files identical despite different names*

### Comparing `glpic-99.0.202405101244/glpic/__init__.py` & `glpic-99.0.202405101247/glpic/__init__.py`

 * *Files identical despite different names*

### Comparing `glpic-99.0.202405101244/glpic/cli.py` & `glpic-99.0.202405101247/glpic/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -107,14 +107,17 @@
     glpic = Glpic(args.url, args.user, args.token, args.debug)
     reservationstable = PrettyTable(["Id", "Item", "Begin", "End", "Comment"])
     for reservation in glpic.list_reservations(overrides=handle_parameters(args.param)):
         _id, begin, end, comment = reservation['id'], reservation['begin'], reservation['end'], reservation['comment']
         comment = fill(comment, width=100)
         reservation_id = reservation['reservationitems_id']
         computer_id = glpic.info_reservation(reservation_id)['items_id']
+        computer_data = glpic.info_computer({'computer': computer_id})
+        if not computer_data:
+            continue
         reservation_name = glpic.info_computer({'computer': computer_id})[0]['Computer.name']
         entry = [_id, reservation_name, begin, end, comment]
         reservationstable.add_row(entry)
     print(reservationstable)
 
 
 def cli():
```

### Comparing `glpic-99.0.202405101244/setup.py` & `glpic-99.0.202405101247/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 description = 'Glpic wrapper'
 long_description = description
 if os.path.exists('README.rst'):
     long_description = open('README.rst').read()
 
 setup(
     name='glpic',
-    version='99.0.202405101244',
+    version='99.0.202405101247',
     include_package_data=True,
     packages=find_packages(),
     zip_safe=False,
     description=description,
     long_description=long_description,
     url='http://github.com/karmab/glpic',
     author='Karim Boumedhel',
```

