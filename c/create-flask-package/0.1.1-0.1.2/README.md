# Comparing `tmp/create_flask_package-0.1.1.tar.gz` & `tmp/create_flask_package-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "create_flask_package-0.1.1.tar", last modified: Fri May 10 08:00:37 2024, max compression
+gzip compressed data, was "create_flask_package-0.1.2.tar", last modified: Fri May 10 08:19:38 2024, max compression
```

## Comparing `create_flask_package-0.1.1.tar` & `create_flask_package-0.1.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-10 08:00:37.768267 create_flask_package-0.1.1/
--rw-rw-rw-   0        0        0      228 2024-05-10 08:00:37.767265 create_flask_package-0.1.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-10 08:00:37.735265 create_flask_package-0.1.1/create_flask_package/
--rw-rw-rw-   0        0        0        0 2024-05-10 05:38:02.000000 create_flask_package-0.1.1/create_flask_package/__init__.py
--rw-rw-rw-   0        0        0     3794 2024-05-10 07:51:58.000000 create_flask_package-0.1.1/create_flask_package/create_flask_package.py
-drwxrwxrwx   0        0        0        0 2024-05-10 08:00:37.766265 create_flask_package-0.1.1/create_flask_package.egg-info/
--rw-rw-rw-   0        0        0      228 2024-05-10 08:00:37.000000 create_flask_package-0.1.1/create_flask_package.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      352 2024-05-10 08:00:37.000000 create_flask_package-0.1.1/create_flask_package.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-10 08:00:37.000000 create_flask_package-0.1.1/create_flask_package.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      107 2024-05-10 08:00:37.000000 create_flask_package-0.1.1/create_flask_package.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       60 2024-05-10 08:00:37.000000 create_flask_package-0.1.1/create_flask_package.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2024-05-10 08:00:37.000000 create_flask_package-0.1.1/create_flask_package.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-10 08:00:37.768267 create_flask_package-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      496 2024-05-10 08:00:05.000000 create_flask_package-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:19:38.850843 create_flask_package-0.1.2/
+-rw-rw-rw-   0        0        0      228 2024-05-10 08:19:38.849840 create_flask_package-0.1.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-10 08:19:38.822874 create_flask_package-0.1.2/create_flask_package/
+-rw-rw-rw-   0        0        0        0 2024-05-10 05:38:02.000000 create_flask_package-0.1.2/create_flask_package/__init__.py
+-rw-rw-rw-   0        0        0     3803 2024-05-10 08:18:46.000000 create_flask_package-0.1.2/create_flask_package/create_flask_package.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:19:38.847840 create_flask_package-0.1.2/create_flask_package.egg-info/
+-rw-rw-rw-   0        0        0      228 2024-05-10 08:19:38.000000 create_flask_package-0.1.2/create_flask_package.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      352 2024-05-10 08:19:38.000000 create_flask_package-0.1.2/create_flask_package.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-10 08:19:38.000000 create_flask_package-0.1.2/create_flask_package.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      110 2024-05-10 08:19:38.000000 create_flask_package-0.1.2/create_flask_package.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       60 2024-05-10 08:19:38.000000 create_flask_package-0.1.2/create_flask_package.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2024-05-10 08:19:38.000000 create_flask_package-0.1.2/create_flask_package.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-10 08:19:38.850843 create_flask_package-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      499 2024-05-10 08:19:04.000000 create_flask_package-0.1.2/setup.py
```

### Comparing `create_flask_package-0.1.1/create_flask_package/create_flask_package.py` & `create_flask_package-0.1.2/create_flask_package/create_flask_package.py`

 * *Files 1% similar despite different names*

```diff
@@ -96,28 +96,28 @@
         f.write('recursive-include {} *.py'.format(package_name))
 
     # Create setup.py
     setup_content = f"""
 from setuptools import setup, find_packages
 
 setup(
-    name='{package_name}',
+    name='create_flask_package',
     version='0.1.1',
     author= 'Nasir Iqbal',
     packages=find_packages(),
     install_requires=[
         'Flask',
         'Flask-SQLAlchemy',
         'Flask-CORS',
         'Flask-Login',
         'Flask-Session'
     ],
     entry_points={
         'console_scripts': [
-            'create_flask_package = your_package_name.create_flask_package:create_package_entry_point'
+            'create_flask_package = create_flask_package.create_flask_package:create_package_entry_point'
         ]
     },
 )
 """
 
     with open('setup.py', 'w') as f:
         f.write(setup_content)
```

