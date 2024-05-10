# Comparing `tmp/containers_sugar-1.9.2.tar.gz` & `tmp/containers_sugar-1.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "containers_sugar-1.9.2.tar", max compression
+gzip compressed data, was "containers_sugar-1.9.3.tar", max compression
```

## Comparing `containers_sugar-1.9.2.tar` & `containers_sugar-1.9.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1514 2023-12-13 02:01:58.506168 containers_sugar-1.9.2/LICENSE
--rw-r--r--   0        0        0     2009 2023-12-13 02:04:45.958230 containers_sugar-1.9.2/pyproject.toml
--rw-r--r--   0        0        0      194 2023-12-13 02:04:45.958230 containers_sugar-1.9.2/src/sugar/__init__.py
--rw-r--r--   0        0        0      124 2023-12-13 02:01:58.510168 containers_sugar-1.9.2/src/sugar/__main__.py
--rw-r--r--   0        0        0     4387 2023-12-13 02:01:58.510168 containers_sugar-1.9.2/src/sugar/cli.py
--rw-r--r--   0        0        0     1074 2023-12-13 02:01:58.510168 containers_sugar-1.9.2/src/sugar/logs.py
--rw-r--r--   0        0        0    17944 2023-12-13 02:01:58.510168 containers_sugar-1.9.2/src/sugar/sugar.py
--rw-r--r--   0        0        0      655 1970-01-01 00:00:00.000000 containers_sugar-1.9.2/PKG-INFO
+-rw-r--r--   0        0        0     1514 2023-12-24 00:27:52.263287 containers_sugar-1.9.3/LICENSE
+-rw-r--r--   0        0        0     1988 2023-12-24 00:30:46.635305 containers_sugar-1.9.3/pyproject.toml
+-rw-r--r--   0        0        0      194 2023-12-24 00:30:46.635305 containers_sugar-1.9.3/src/sugar/__init__.py
+-rw-r--r--   0        0        0      124 2023-12-24 00:27:52.263287 containers_sugar-1.9.3/src/sugar/__main__.py
+-rw-r--r--   0        0        0     4387 2023-12-24 00:27:52.263287 containers_sugar-1.9.3/src/sugar/cli.py
+-rw-r--r--   0        0        0     1074 2023-12-24 00:27:52.267287 containers_sugar-1.9.3/src/sugar/logs.py
+-rw-r--r--   0        0        0    18184 2023-12-24 00:27:52.267287 containers_sugar-1.9.3/src/sugar/sugar.py
+-rw-r--r--   0        0        0      672 1970-01-01 00:00:00.000000 containers_sugar-1.9.3/PKG-INFO
```

### Comparing `containers_sugar-1.9.2/LICENSE` & `containers_sugar-1.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `containers_sugar-1.9.2/pyproject.toml` & `containers_sugar-1.9.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "containers-sugar"
-version = "1.9.2"  # semantic-release
+version = "1.9.3"  # semantic-release
 description = "Simplify the usage of containers"
 authors = ["Ivan Ogasawara <ivan.ogasawara@gmail.com>"]
 license = "BSD 3 Clause"
 packages = [
   {include = "sugar", from="src"},
 ]
 include = ["src/sugar/py.typed"]
@@ -13,21 +13,20 @@
   ".env*",
 ]
 
 [tool.poetry.scripts]
 "sugar" = "sugar.__main__:app"
 
 [tool.poetry.dependencies]
-python = ">=3.8.1,<3.12"
+python = ">=3.8.1,<4"
 Jinja2 = ">=2"
 sh = ">=2.0.0"
 pyyaml = ">=6"
 colorama = ">=0.4.6"
 python-dotenv = ">=0.21.1"
-distlib = ">=0.3"
 
 [tool.poetry.group.dev.dependencies]
 pytest = ">=7.3.2"
 pytest-cov = ">=4.1.0"
 coverage = ">=7.2.7"
 pre-commit = ">=3.3.2"
 ruff = ">=0.1.5"
```

### Comparing `containers_sugar-1.9.2/src/sugar/cli.py` & `containers_sugar-1.9.3/src/sugar/cli.py`

 * *Files identical despite different names*

### Comparing `containers_sugar-1.9.2/src/sugar/logs.py` & `containers_sugar-1.9.3/src/sugar/logs.py`

 * *Files identical despite different names*

### Comparing `containers_sugar-1.9.2/src/sugar/sugar.py` & `containers_sugar-1.9.3/src/sugar/sugar.py`

 * *Files 2% similar despite different names*

```diff
@@ -125,34 +125,38 @@
             default_group = self.defaults.get('group')
             if not default_group:
                 KxgrLogs.raise_error(
                     'The service group parameter or default '
                     "group configuration weren't defined.",
                     KxgrErrorType.KXGR_INVALID_PARAMETER,
                 )
-            group_name = default_group
+            selected_group_name = default_group
         else:
-            group_name = self.args.get('service_group')
+            selected_group_name = self.args.get('service_group')
 
         default_project_name = self.defaults.get('project-name')
 
-        for g in groups:
-            if g['name'] == group_name:
-                if default_project_name and 'project-name' not in g:
+        for group_name, group_data in groups.items():
+            if group_name == selected_group_name:
+                if default_project_name and 'project-name' not in group_data:
                     # just use default value if "project-name" is not set
-                    g['project-name'] = default_project_name
-                if not g.get('services', {}).get('default'):
+                    group_data['project-name'] = default_project_name
+                if not group_data.get('services', {}).get('default'):
                     # if default is not given or it is empty or null,
                     # use as default all the services available
                     default_services = [
                         service['name']
-                        for service in g.get('services', {}).get('available')
+                        for service in group_data.get('services', {}).get(
+                            'available'
+                        )
                     ]
-                    g['services']['default'] = ','.join(default_services)
-                self.service_group = g
+                    group_data['services']['default'] = ','.join(
+                        default_services
+                    )
+                self.service_group = group_data
                 return
 
         KxgrLogs.raise_error(
             f'The given group service "{group_name}" was not found '
             'in the configuration file.',
             KxgrErrorType.KXGR_MISSING_PARAMETER,
         )
@@ -362,15 +366,15 @@
         super().__init__(*args, **kwargs)
 
     # container commands
     def _build(self):
         self._call_compose_app('build', services=self.service_names)
 
     def _config(self):
-        self._call_compose_app('config')
+        self._call_compose_app('config', services=self.service_names)
 
     def _create(self):
         self._call_compose_app('create', services=self.service_names)
 
     def _down(self):
         if self.args.get('all') or self.args.get('services'):
             KxgrLogs.raise_error(
```

