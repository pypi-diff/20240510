# Comparing `tmp/digitalmarketplace-developer-tools-1.1.0rc2.tar.gz` & `tmp/digitalmarketplace-developer-tools-1.1.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "digitalmarketplace-developer-tools-1.1.0rc2.tar", last modified: Tue Feb 20 08:57:08 2024, max compression
+gzip compressed data, was "digitalmarketplace-developer-tools-1.1.0rc3.tar", last modified: Fri May 10 14:25:16 2024, max compression
```

## Comparing `digitalmarketplace-developer-tools-1.1.0rc2.tar` & `digitalmarketplace-developer-tools-1.1.0rc3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 08:57:08.884439 digitalmarketplace-developer-tools-1.1.0rc2/
--rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-02-20 08:57:00.000000 digitalmarketplace-developer-tools-1.1.0rc2/LICENCE
--rw-r--r--   0 runner    (1001) docker     (127)     2637 2024-02-20 08:57:08.884439 digitalmarketplace-developer-tools-1.1.0rc2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2256 2024-02-20 08:57:00.000000 digitalmarketplace-developer-tools-1.1.0rc2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 08:57:08.884439 digitalmarketplace-developer-tools-1.1.0rc2/digitalmarketplace_developer_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2637 2024-02-20 08:57:08.000000 digitalmarketplace-developer-tools-1.1.0rc2/digitalmarketplace_developer_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-02-20 08:57:08.000000 digitalmarketplace-developer-tools-1.1.0rc2/digitalmarketplace_developer_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-20 08:57:08.000000 digitalmarketplace-developer-tools-1.1.0rc2/digitalmarketplace_developer_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-02-20 08:57:08.000000 digitalmarketplace-developer-tools-1.1.0rc2/digitalmarketplace_developer_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-02-20 08:57:08.000000 digitalmarketplace-developer-tools-1.1.0rc2/digitalmarketplace_developer_tools.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 08:57:08.884439 digitalmarketplace-developer-tools-1.1.0rc2/dmdevtools/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-02-20 08:57:00.000000 digitalmarketplace-developer-tools-1.1.0rc2/dmdevtools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7330 2024-02-20 08:57:00.000000 digitalmarketplace-developer-tools-1.1.0rc2/dmdevtools/invoke_tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-20 08:57:08.884439 digitalmarketplace-developer-tools-1.1.0rc2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      936 2024-02-20 08:57:00.000000 digitalmarketplace-developer-tools-1.1.0rc2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:25:16.120614 digitalmarketplace-developer-tools-1.1.0rc3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-05-10 14:25:07.000000 digitalmarketplace-developer-tools-1.1.0rc3/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (127)     2637 2024-05-10 14:25:16.120614 digitalmarketplace-developer-tools-1.1.0rc3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2256 2024-05-10 14:25:07.000000 digitalmarketplace-developer-tools-1.1.0rc3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:25:16.120614 digitalmarketplace-developer-tools-1.1.0rc3/digitalmarketplace_developer_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2637 2024-05-10 14:25:16.000000 digitalmarketplace-developer-tools-1.1.0rc3/digitalmarketplace_developer_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-05-10 14:25:16.000000 digitalmarketplace-developer-tools-1.1.0rc3/digitalmarketplace_developer_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 14:25:16.000000 digitalmarketplace-developer-tools-1.1.0rc3/digitalmarketplace_developer_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-10 14:25:16.000000 digitalmarketplace-developer-tools-1.1.0rc3/digitalmarketplace_developer_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-10 14:25:16.000000 digitalmarketplace-developer-tools-1.1.0rc3/digitalmarketplace_developer_tools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:25:16.120614 digitalmarketplace-developer-tools-1.1.0rc3/dmdevtools/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-10 14:25:07.000000 digitalmarketplace-developer-tools-1.1.0rc3/dmdevtools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6888 2024-05-10 14:25:07.000000 digitalmarketplace-developer-tools-1.1.0rc3/dmdevtools/invoke_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 14:25:16.120614 digitalmarketplace-developer-tools-1.1.0rc3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      936 2024-05-10 14:25:07.000000 digitalmarketplace-developer-tools-1.1.0rc3/setup.py
```

### Comparing `digitalmarketplace-developer-tools-1.1.0rc2/LICENCE` & `digitalmarketplace-developer-tools-1.1.0rc3/LICENCE`

 * *Files identical despite different names*

### Comparing `digitalmarketplace-developer-tools-1.1.0rc2/PKG-INFO` & `digitalmarketplace-developer-tools-1.1.0rc3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: digitalmarketplace-developer-tools
-Version: 1.1.0rc2
+Version: 1.1.0rc3
 Summary: Common developer tools for Digital Marketplace repos
 Home-page: https://github.com/Crown-Commercial-Service/digitalmarketplace-developer-tools
 Author: GDS Developers
 License: MIT
 Platform: UNKNOWN
 Requires-Python: >=3.9,<3.13
 Description-Content-Type: text/markdown
```

### Comparing `digitalmarketplace-developer-tools-1.1.0rc2/README.md` & `digitalmarketplace-developer-tools-1.1.0rc3/README.md`

 * *Files identical despite different names*

### Comparing `digitalmarketplace-developer-tools-1.1.0rc2/digitalmarketplace_developer_tools.egg-info/PKG-INFO` & `digitalmarketplace-developer-tools-1.1.0rc3/digitalmarketplace_developer_tools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: digitalmarketplace-developer-tools
-Version: 1.1.0rc2
+Version: 1.1.0rc3
 Summary: Common developer tools for Digital Marketplace repos
 Home-page: https://github.com/Crown-Commercial-Service/digitalmarketplace-developer-tools
 Author: GDS Developers
 License: MIT
 Platform: UNKNOWN
 Requires-Python: >=3.9,<3.13
 Description-Content-Type: text/markdown
```

### Comparing `digitalmarketplace-developer-tools-1.1.0rc2/dmdevtools/invoke_tasks.py` & `digitalmarketplace-developer-tools-1.1.0rc3/dmdevtools/invoke_tasks.py`

 * *Files 4% similar despite different names*

```diff
@@ -168,21 +168,15 @@
 
     c.run(f"docker push {repo_name}:{release_name}")
 
 
 @task(show_environment, virtualenv)
 def run_app(c):
     """Run app"""
-    c.run("flask run")
-
-
-@task(show_environment, virtualenv)
-def run_app_debug(c):
-    """Run app [In DEBUG mode]"""
-    c.run("flask --debug run")
+    c.run("flask run --debug")
 
 
 # Create collections for each kind of repo
 # This probably isn't the best way to do this,
 # but it seems to work.
 _common_tasks = [
     virtualenv,
@@ -194,15 +188,14 @@
     test_mypy,
     test_python,
     show_environment,
 ]
 _common_app_tasks = [
     *_common_tasks,
     run_app,
-    run_app_debug,
     docker_build,
     docker_push,
 ]
 _common_configuration = {
     "run": {"echo": True, "pty": True}  # set commands to echo like in Make by default
 }
 
@@ -226,15 +219,14 @@
     *_common_tasks,
     _empty_task(test_flake8, test_python, name="test", doc="Run all tests"),
 )
 
 api_app_tasks = _Collection(
     *_common_app_tasks,
     _empty_task(requirements_dev, run_app, name="run-all", doc="Build and run app"),
-    _empty_task(requirements_dev, run_app_debug, name="run-all-debug", doc="Build and run app in debug mode"),
     _empty_task(test_flake8, test_python, name="test", doc="Run all tests"),
 )
 
 frontend_app_tasks = _Collection(
     *_common_app_tasks,
     npm_install,
     frontend_build,
@@ -243,22 +235,14 @@
         npm_install,
         frontend_build,
         run_app,
         name="run-all",
         doc="Build and run app",
     ),
     _empty_task(
-        requirements_dev,
-        npm_install,
-        frontend_build,
-        run_app_debug,
-        name="run-all-debug",
-        doc="Build and run app in debug mode",
-    ),
-    _empty_task(
         show_environment,
         frontend_build,
         test_flake8,
         test_python,
         test_javascript,
         name="test",
     ),
```

### Comparing `digitalmarketplace-developer-tools-1.1.0rc2/setup.py` & `digitalmarketplace-developer-tools-1.1.0rc3/setup.py`

 * *Files identical despite different names*

