# Comparing `tmp/create_flask_package-0.1.2.tar.gz` & `tmp/create_flask_package-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "create_flask_package-0.1.2.tar", last modified: Fri May 10 08:19:38 2024, max compression
+gzip compressed data, was "create_flask_package-0.1.3.tar", last modified: Fri May 10 08:30:40 2024, max compression
```

## Comparing `create_flask_package-0.1.2.tar` & `create_flask_package-0.1.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-10 08:19:38.850843 create_flask_package-0.1.2/
--rw-rw-rw-   0        0        0      228 2024-05-10 08:19:38.849840 create_flask_package-0.1.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-10 08:19:38.822874 create_flask_package-0.1.2/create_flask_package/
--rw-rw-rw-   0        0        0        0 2024-05-10 05:38:02.000000 create_flask_package-0.1.2/create_flask_package/__init__.py
--rw-rw-rw-   0        0        0     3803 2024-05-10 08:18:46.000000 create_flask_package-0.1.2/create_flask_package/create_flask_package.py
-drwxrwxrwx   0        0        0        0 2024-05-10 08:19:38.847840 create_flask_package-0.1.2/create_flask_package.egg-info/
--rw-rw-rw-   0        0        0      228 2024-05-10 08:19:38.000000 create_flask_package-0.1.2/create_flask_package.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      352 2024-05-10 08:19:38.000000 create_flask_package-0.1.2/create_flask_package.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-10 08:19:38.000000 create_flask_package-0.1.2/create_flask_package.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      110 2024-05-10 08:19:38.000000 create_flask_package-0.1.2/create_flask_package.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       60 2024-05-10 08:19:38.000000 create_flask_package-0.1.2/create_flask_package.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2024-05-10 08:19:38.000000 create_flask_package-0.1.2/create_flask_package.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-10 08:19:38.850843 create_flask_package-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      499 2024-05-10 08:19:04.000000 create_flask_package-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:30:40.662069 create_flask_package-0.1.3/
+-rw-rw-rw-   0        0        0      228 2024-05-10 08:30:40.659072 create_flask_package-0.1.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-10 08:30:40.617334 create_flask_package-0.1.3/create_flask_package/
+-rw-rw-rw-   0        0        0        0 2024-05-10 05:38:02.000000 create_flask_package-0.1.3/create_flask_package/__init__.py
+-rw-rw-rw-   0        0        0     3175 2024-05-10 08:27:41.000000 create_flask_package-0.1.3/create_flask_package/create_flask_package.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:30:40.657067 create_flask_package-0.1.3/create_flask_package.egg-info/
+-rw-rw-rw-   0        0        0      228 2024-05-10 08:30:40.000000 create_flask_package-0.1.3/create_flask_package.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      352 2024-05-10 08:30:40.000000 create_flask_package-0.1.3/create_flask_package.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-10 08:30:40.000000 create_flask_package-0.1.3/create_flask_package.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      110 2024-05-10 08:30:40.000000 create_flask_package-0.1.3/create_flask_package.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       60 2024-05-10 08:30:40.000000 create_flask_package-0.1.3/create_flask_package.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2024-05-10 08:30:40.000000 create_flask_package-0.1.3/create_flask_package.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-10 08:30:40.663073 create_flask_package-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      499 2024-05-10 08:30:37.000000 create_flask_package-0.1.3/setup.py
```

### Comparing `create_flask_package-0.1.2/create_flask_package/create_flask_package.py` & `create_flask_package-0.1.3/create_flask_package/create_flask_package.py`

 * *Files 8% similar despite different names*

```diff
@@ -91,40 +91,13 @@
     application.run(debug=True, host="0.0.0.0")
     ''')
 
     # Create MANIFEST.in
     with open('MANIFEST.in', 'w') as f:
         f.write('recursive-include {} *.py'.format(package_name))
 
-    # Create setup.py
-    setup_content = f"""
-from setuptools import setup, find_packages
-
-setup(
-    name='create_flask_package',
-    version='0.1.1',
-    author= 'Nasir Iqbal',
-    packages=find_packages(),
-    install_requires=[
-        'Flask',
-        'Flask-SQLAlchemy',
-        'Flask-CORS',
-        'Flask-Login',
-        'Flask-Session'
-    ],
-    entry_points={
-        'console_scripts': [
-            'create_flask_package = create_flask_package.create_flask_package:create_package_entry_point'
-        ]
-    },
-)
-"""
-
-    with open('setup.py', 'w') as f:
-        f.write(setup_content)
-
 def create_package_entry_point():
     package_name = input("Enter the name of your package: ")
     create_package(package_name)
 
 if __name__ == "__main__":
     create_package_entry_point()
```

