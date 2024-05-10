# Comparing `tmp/flask-allowedhosts-1.2.0.tar.gz` & `tmp/flask_allowedhosts-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask-allowedhosts-1.2.0.tar", last modified: Wed Jul 19 16:11:44 2023, max compression
+gzip compressed data, was "flask_allowedhosts-1.3.0.tar", last modified: Fri May 10 19:56:04 2024, max compression
```

## Comparing `flask-allowedhosts-1.2.0.tar` & `flask_allowedhosts-1.3.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-19 16:11:44.080399 flask-allowedhosts-1.2.0/
--rw-rw-rw-   0        0        0     1090 2023-06-24 09:14:27.000000 flask-allowedhosts-1.2.0/LICENSE.md
--rw-rw-rw-   0        0        0     2538 2023-07-19 16:11:44.079375 flask-allowedhosts-1.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     1598 2023-07-19 16:09:10.000000 flask-allowedhosts-1.2.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-19 16:11:44.052377 flask-allowedhosts-1.2.0/flask_allowedhosts/
--rw-rw-rw-   0        0        0       36 2023-07-19 16:08:44.000000 flask-allowedhosts-1.2.0/flask_allowedhosts/__init__.py
--rw-rw-rw-   0        0        0     1567 2023-07-19 16:01:28.000000 flask-allowedhosts-1.2.0/flask_allowedhosts/decorators.py
--rw-rw-rw-   0        0        0      274 2023-07-19 16:00:47.000000 flask-allowedhosts-1.2.0/flask_allowedhosts/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-19 16:11:44.078427 flask-allowedhosts-1.2.0/flask_allowedhosts.egg-info/
--rw-rw-rw-   0        0        0     2538 2023-07-19 16:11:43.000000 flask-allowedhosts-1.2.0/flask_allowedhosts.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      330 2023-07-19 16:11:43.000000 flask-allowedhosts-1.2.0/flask_allowedhosts.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-19 16:11:43.000000 flask-allowedhosts-1.2.0/flask_allowedhosts.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-07-19 16:11:43.000000 flask-allowedhosts-1.2.0/flask_allowedhosts.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-07-19 16:11:43.000000 flask-allowedhosts-1.2.0/flask_allowedhosts.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-19 16:11:44.080399 flask-allowedhosts-1.2.0/setup.cfg
--rw-rw-rw-   0        0        0     1170 2023-07-19 16:10:52.000000 flask-allowedhosts-1.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-10 19:56:04.531437 flask_allowedhosts-1.3.0/
+-rw-rw-rw-   0        0        0     1090 2024-05-10 19:01:04.000000 flask_allowedhosts-1.3.0/LICENSE.md
+-rw-rw-rw-   0        0        0     2887 2024-05-10 19:56:04.531437 flask_allowedhosts-1.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1978 2024-05-10 19:47:01.000000 flask_allowedhosts-1.3.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-10 19:56:04.523920 flask_allowedhosts-1.3.0/flask_allowedhosts/
+-rw-rw-rw-   0        0        0       37 2024-05-10 19:01:04.000000 flask_allowedhosts-1.3.0/flask_allowedhosts/__init__.py
+-rw-rw-rw-   0        0        0     1772 2024-05-10 19:50:19.000000 flask_allowedhosts-1.3.0/flask_allowedhosts/decorators.py
+-rw-rw-rw-   0        0        0      290 2024-05-10 19:49:43.000000 flask_allowedhosts-1.3.0/flask_allowedhosts/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-10 19:56:04.530436 flask_allowedhosts-1.3.0/flask_allowedhosts.egg-info/
+-rw-rw-rw-   0        0        0     2887 2024-05-10 19:56:04.000000 flask_allowedhosts-1.3.0/flask_allowedhosts.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      330 2024-05-10 19:56:04.000000 flask_allowedhosts-1.3.0/flask_allowedhosts.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-10 19:56:04.000000 flask_allowedhosts-1.3.0/flask_allowedhosts.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2024-05-10 19:56:04.000000 flask_allowedhosts-1.3.0/flask_allowedhosts.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2024-05-10 19:56:04.000000 flask_allowedhosts-1.3.0/flask_allowedhosts.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-10 19:56:04.531437 flask_allowedhosts-1.3.0/setup.cfg
+-rw-rw-rw-   0        0        0     1201 2024-05-10 19:15:07.000000 flask_allowedhosts-1.3.0/setup.py
```

### Comparing `flask-allowedhosts-1.2.0/LICENSE.md` & `flask_allowedhosts-1.3.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `flask-allowedhosts-1.2.0/PKG-INFO` & `flask_allowedhosts-1.3.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,28 +1,7 @@
-Metadata-Version: 2.1
-Name: flask-allowedhosts
-Version: 1.2.0
-Summary: A Flask extension to limit access to your routes by using allowed hosts.
-Home-page: https://github.com/riad-azz/flask-allowedhosts
-Author: Riadh Azzoun
-Author-email: riadh.azzoun@hotmail.com
-License: MIT
-Keywords: flask,allowed hosts,web development,security
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
-Classifier: Topic :: Internet :: WWW/HTTP :: WSGI :: Application
-Classifier: Topic :: Security
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-License-File: LICENSE.md
-
 # Flask Allowed Hosts
 
 Flask Allowed Hosts is a Flask extension that provides host validation for API endpoints. It allows you to enforce that requests are only accepted from specific hosts, providing an additional layer of security for your Flask application.
 
 ## Installation
 
 Install the package using pip:
@@ -43,30 +22,36 @@
 from flask import Flask, request, jsonify
 from flask_allowedhosts import limit_hosts
 
 app = Flask(__name__)
 
 ALLOWED_HOSTS = ['127.0.0.1', 'localhost']
 
+def on_denied():
+    return "Unauthorized access", 401
 
 @app.route("/api/greet")
-@limit_hosts(allowed_hosts=ALLOWED_HOSTS)
+@limit_hosts(allowed_hosts=ALLOWED_HOSTS, on_denied=on_denied)
 def greet_endpoint():
     name = request.args.get("name", "Friend")
     greeting = {"greeting": f"Hello There {name}!"}
     return jsonify(greeting), 200
 
 
 if __name__ == '__main__':
     app.run(host='0.0.0.0', port=5000)
 ```
 
 Now only the allowed hosts set in `ALLOWED_HOSTS` can access the protected endpoint(s). Requests from other hosts will receive a 403 Forbidden error.
 
-_The default value for `allowed_hosts` is an empty list, which means requests from all hosts are allowed._
+### Arguments
+
+- `allowed_hosts`: List[str] : Modify this list to include the allowed hosts. The default value is an empty list `[]`, which means requests from all hosts are allowed.
+
+- `on_denied`: Callable: Modify this function to customize the behavior when a request is denied. The default is `None`, which means a 403 Forbidden error is returned.
 
 ## Contributing
 
 Contributions are welcome! If you have any suggestions, bug reports, or feature requests, please open an issue or submit a pull request.
 
 ## License
```

### Comparing `flask-allowedhosts-1.2.0/flask_allowedhosts.egg-info/PKG-INFO` & `flask_allowedhosts-1.3.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-allowedhosts
-Version: 1.2.0
+Version: 1.3.0
 Summary: A Flask extension to limit access to your routes by using allowed hosts.
 Home-page: https://github.com/riad-azz/flask-allowedhosts
 Author: Riadh Azzoun
 Author-email: riadh.azzoun@hotmail.com
 License: MIT
 Keywords: flask,allowed hosts,web development,security
 Classifier: Development Status :: 5 - Production/Stable
@@ -14,14 +14,15 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI :: Application
 Classifier: Topic :: Security
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
+Requires-Dist: Flask
 
 # Flask Allowed Hosts
 
 Flask Allowed Hosts is a Flask extension that provides host validation for API endpoints. It allows you to enforce that requests are only accepted from specific hosts, providing an additional layer of security for your Flask application.
 
 ## Installation
 
@@ -43,30 +44,36 @@
 from flask import Flask, request, jsonify
 from flask_allowedhosts import limit_hosts
 
 app = Flask(__name__)
 
 ALLOWED_HOSTS = ['127.0.0.1', 'localhost']
 
+def on_denied():
+    return "Unauthorized access", 401
 
 @app.route("/api/greet")
-@limit_hosts(allowed_hosts=ALLOWED_HOSTS)
+@limit_hosts(allowed_hosts=ALLOWED_HOSTS, on_denied=on_denied)
 def greet_endpoint():
     name = request.args.get("name", "Friend")
     greeting = {"greeting": f"Hello There {name}!"}
     return jsonify(greeting), 200
 
 
 if __name__ == '__main__':
     app.run(host='0.0.0.0', port=5000)
 ```
 
 Now only the allowed hosts set in `ALLOWED_HOSTS` can access the protected endpoint(s). Requests from other hosts will receive a 403 Forbidden error.
 
-_The default value for `allowed_hosts` is an empty list, which means requests from all hosts are allowed._
+### Arguments
+
+- `allowed_hosts`: List[str] : Modify this list to include the allowed hosts. The default value is an empty list `[]`, which means requests from all hosts are allowed.
+
+- `on_denied`: Callable: Modify this function to customize the behavior when a request is denied. The default is `None`, which means a 403 Forbidden error is returned.
 
 ## Contributing
 
 Contributions are welcome! If you have any suggestions, bug reports, or feature requests, please open an issue or submit a pull request.
 
 ## License
```

### Comparing `flask-allowedhosts-1.2.0/setup.py` & `flask_allowedhosts-1.3.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,32 +1,32 @@
-from setuptools import setup
-
-long_description = open('README.md').read()
-long_description_content_type = 'text/markdown'
-
-setup(
-    name='flask-allowedhosts',
-    version='1.2.0',
-    packages=['flask_allowedhosts'],
-    install_requires=[
-        'Flask',
-    ],
-    url='https://github.com/riad-azz/flask-allowedhosts',
-    license='MIT',
-    author='Riadh Azzoun',
-    author_email='riadh.azzoun@hotmail.com',
-    description='A Flask extension to limit access to your routes by using allowed hosts.',
-    long_description=long_description,
-    long_description_content_type=long_description_content_type,
-    keywords=["flask", "allowed hosts", "web development", "security"],
-    classifiers=[
-        "Development Status :: 5 - Production/Stable",
-        "Intended Audience :: Developers",
-        "License :: OSI Approved :: MIT License",
-        "Programming Language :: Python",
-        "Topic :: Software Development :: Libraries :: Python Modules",
-        "Topic :: Internet :: WWW/HTTP :: Dynamic Content",
-        "Topic :: Internet :: WWW/HTTP :: WSGI :: Application",
-        "Topic :: Security",
-        "Operating System :: OS Independent",
-    ],
+from setuptools import setup
+
+long_description = open('README.md').read()
+long_description_content_type = 'text/markdown'
+
+setup(
+    name='flask-allowedhosts',
+    version='1.3.0',
+    packages=['flask_allowedhosts'],
+    install_requires=[
+        'Flask',
+    ],
+    url='https://github.com/riad-azz/flask-allowedhosts',
+    license='MIT',
+    author='Riadh Azzoun',
+    author_email='riadh.azzoun@hotmail.com',
+    description='A Flask extension to limit access to your routes by using allowed hosts.',
+    long_description=long_description,
+    long_description_content_type=long_description_content_type,
+    keywords=["flask", "allowed hosts", "web development", "security"],
+    classifiers=[
+        "Development Status :: 5 - Production/Stable",
+        "Intended Audience :: Developers",
+        "License :: OSI Approved :: MIT License",
+        "Programming Language :: Python",
+        "Topic :: Software Development :: Libraries :: Python Modules",
+        "Topic :: Internet :: WWW/HTTP :: Dynamic Content",
+        "Topic :: Internet :: WWW/HTTP :: WSGI :: Application",
+        "Topic :: Security",
+        "Operating System :: OS Independent",
+    ],
 )
```

