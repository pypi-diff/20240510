# Comparing `tmp/create_flask_package-0.1.4.tar.gz` & `tmp/create_flask_package-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "create_flask_package-0.1.4.tar", last modified: Fri May 10 08:48:13 2024, max compression
+gzip compressed data, was "create_flask_package-0.1.5.tar", last modified: Fri May 10 09:32:00 2024, max compression
```

## Comparing `create_flask_package-0.1.4.tar` & `create_flask_package-0.1.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-10 08:48:13.135310 create_flask_package-0.1.4/
--rw-rw-rw-   0        0        0      228 2024-05-10 08:48:13.134316 create_flask_package-0.1.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-10 08:48:13.106346 create_flask_package-0.1.4/create_flask_package/
--rw-rw-rw-   0        0        0        0 2024-05-10 05:38:02.000000 create_flask_package-0.1.4/create_flask_package/__init__.py
--rw-rw-rw-   0        0        0     3440 2024-05-10 08:47:58.000000 create_flask_package-0.1.4/create_flask_package/create_flask_package.py
-drwxrwxrwx   0        0        0        0 2024-05-10 08:48:13.133312 create_flask_package-0.1.4/create_flask_package.egg-info/
--rw-rw-rw-   0        0        0      228 2024-05-10 08:48:12.000000 create_flask_package-0.1.4/create_flask_package.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      352 2024-05-10 08:48:13.000000 create_flask_package-0.1.4/create_flask_package.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-10 08:48:13.000000 create_flask_package-0.1.4/create_flask_package.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      110 2024-05-10 08:48:13.000000 create_flask_package-0.1.4/create_flask_package.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       60 2024-05-10 08:48:13.000000 create_flask_package-0.1.4/create_flask_package.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2024-05-10 08:48:13.000000 create_flask_package-0.1.4/create_flask_package.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-10 08:48:13.135310 create_flask_package-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0      499 2024-05-10 08:48:04.000000 create_flask_package-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-10 09:32:00.639724 create_flask_package-0.1.5/
+-rw-rw-rw-   0        0        0      259 2024-05-10 09:32:00.637724 create_flask_package-0.1.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-10 09:32:00.610728 create_flask_package-0.1.5/create_flask_package/
+-rw-rw-rw-   0        0        0        0 2024-05-10 05:38:02.000000 create_flask_package-0.1.5/create_flask_package/__init__.py
+-rw-rw-rw-   0        0        0     3463 2024-05-10 09:31:44.000000 create_flask_package-0.1.5/create_flask_package/create_flask_package.py
+drwxrwxrwx   0        0        0        0 2024-05-10 09:32:00.635722 create_flask_package-0.1.5/create_flask_package.egg-info/
+-rw-rw-rw-   0        0        0      259 2024-05-10 09:32:00.000000 create_flask_package-0.1.5/create_flask_package.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      352 2024-05-10 09:32:00.000000 create_flask_package-0.1.5/create_flask_package.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-10 09:32:00.000000 create_flask_package-0.1.5/create_flask_package.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      110 2024-05-10 09:32:00.000000 create_flask_package-0.1.5/create_flask_package.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       60 2024-05-10 09:32:00.000000 create_flask_package-0.1.5/create_flask_package.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2024-05-10 09:32:00.000000 create_flask_package-0.1.5/create_flask_package.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-10 09:32:00.639724 create_flask_package-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0     2716 2024-05-10 09:31:01.000000 create_flask_package-0.1.5/setup.py
```

### Comparing `create_flask_package-0.1.4/create_flask_package/create_flask_package.py` & `create_flask_package-0.1.5/create_flask_package/create_flask_package.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 
     init_content = f"""
 from flask import Flask
 from flask_sqlalchemy import SQLAlchemy
 from flask_login import LoginManager
 from flask_session import Session
 from flask_cors import CORS
-import os
 
 db = SQLAlchemy()
 app = Flask(__name__, static_url_path='/static', static_folder='static')
 app.config["SECRET_KEY"] = 'your key'
 app.config["SESSION_TYPE"] = "sqlalchemy"
 app.config["SESSION_COOKIE_SAMESITE"] = "Lax"
 app.config['SESSION_SQLALCHEMY'] = db
@@ -87,33 +86,33 @@
 
 application, db = create_app()
 
 if __name__ == "__main__":
     application.run(debug=True, host="0.0.0.0")
     ''')
 
-    # Create setup.py
-    setup_content = f"""
-from setuptools import setup, find_packages
-
-setup(
-    name='create_flask_package',
-    packages=find_packages(),
-    install_requires=[
-        'Flask',
-        'Flask-SQLAlchemy',
-        'Flask-CORS',
-        'Flask-Login',
-        'Flask-Session'
-    ]
-)
-"""
+#     # Create setup.py
+#     setup_content = f"""
+# from setuptools import setup, find_packages
+
+# setup(
+#     name='create_flask_package',
+#     packages=find_packages(),
+#     install_requires=[
+#         'Flask',
+#         'Flask-SQLAlchemy',
+#         'Flask-CORS',
+#         'Flask-Login',
+#         'Flask-Session'
+#     ]
+# )
+# """
 
-    with open('setup.py', 'w') as f:
-        f.write(setup_content)
+#     with open('setup.py', 'w') as f:
+#         f.write(setup_content)
 
 def create_package_entry_point():
     package_name = input("Enter the name of your package: ")
     create_package(package_name)
 
 if __name__ == "__main__":
     create_package_entry_point()
```

