# Comparing `tmp/sparecores_runner-0.0.1.tar.gz` & `tmp/sparecores_runner-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sparecores_runner-0.0.1.tar", last modified: Wed May  1 20:17:20 2024, max compression
+gzip compressed data, was "sparecores_runner-0.0.2.tar", last modified: Fri May 10 20:32:02 2024, max compression
```

## Comparing `sparecores_runner-0.0.1.tar` & `sparecores_runner-0.0.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 20:17:20.411147 sparecores_runner-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)    16725 2024-05-01 20:17:16.000000 sparecores_runner-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      963 2024-05-01 20:17:20.411147 sparecores_runner-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-01 20:17:16.000000 sparecores_runner-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-05-01 20:17:16.000000 sparecores_runner-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 20:17:20.411147 sparecores_runner-0.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 20:17:20.407148 sparecores_runner-0.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 20:17:20.407148 sparecores_runner-0.0.1/src/sc_runner/
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-05-01 20:17:16.000000 sparecores_runner-0.0.1/src/sc_runner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2347 2024-05-01 20:17:16.000000 sparecores_runner-0.0.1/src/sc_runner/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-05-01 20:17:16.000000 sparecores_runner-0.0.1/src/sc_runner/data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 20:17:20.407148 sparecores_runner-0.0.1/src/sc_runner/resources/
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-01 20:17:16.000000 sparecores_runner-0.0.1/src/sc_runner/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7121 2024-05-01 20:17:16.000000 sparecores_runner-0.0.1/src/sc_runner/resources/aws.py
--rw-r--r--   0 runner    (1001) docker     (127)      617 2024-05-01 20:17:16.000000 sparecores_runner-0.0.1/src/sc_runner/resources/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2753 2024-05-01 20:17:16.000000 sparecores_runner-0.0.1/src/sc_runner/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 20:17:20.411147 sparecores_runner-0.0.1/src/sparecores_runner.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      963 2024-05-01 20:17:20.000000 sparecores_runner-0.0.1/src/sparecores_runner.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      496 2024-05-01 20:17:20.000000 sparecores_runner-0.0.1/src/sparecores_runner.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 20:17:20.000000 sparecores_runner-0.0.1/src/sparecores_runner.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-01 20:17:20.000000 sparecores_runner-0.0.1/src/sparecores_runner.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-01 20:17:20.000000 sparecores_runner-0.0.1/src/sparecores_runner.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-01 20:17:20.000000 sparecores_runner-0.0.1/src/sparecores_runner.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:32:02.341211 sparecores_runner-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    16725 2024-05-10 20:31:58.000000 sparecores_runner-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-05-10 20:32:02.341211 sparecores_runner-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-10 20:31:58.000000 sparecores_runner-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-05-10 20:31:58.000000 sparecores_runner-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 20:32:02.341211 sparecores_runner-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:32:02.337211 sparecores_runner-0.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:32:02.337211 sparecores_runner-0.0.2/src/sc_runner/
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-05-10 20:31:58.000000 sparecores_runner-0.0.2/src/sc_runner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2347 2024-05-10 20:31:58.000000 sparecores_runner-0.0.2/src/sc_runner/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-05-10 20:31:58.000000 sparecores_runner-0.0.2/src/sc_runner/data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:32:02.337211 sparecores_runner-0.0.2/src/sc_runner/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-10 20:31:58.000000 sparecores_runner-0.0.2/src/sc_runner/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7121 2024-05-10 20:31:58.000000 sparecores_runner-0.0.2/src/sc_runner/resources/aws.py
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2024-05-10 20:31:58.000000 sparecores_runner-0.0.2/src/sc_runner/resources/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2757 2024-05-10 20:31:58.000000 sparecores_runner-0.0.2/src/sc_runner/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:32:02.341211 sparecores_runner-0.0.2/src/sparecores_runner.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-05-10 20:32:02.000000 sparecores_runner-0.0.2/src/sparecores_runner.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2024-05-10 20:32:02.000000 sparecores_runner-0.0.2/src/sparecores_runner.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 20:32:02.000000 sparecores_runner-0.0.2/src/sparecores_runner.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-10 20:32:02.000000 sparecores_runner-0.0.2/src/sparecores_runner.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-10 20:32:02.000000 sparecores_runner-0.0.2/src/sparecores_runner.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-10 20:32:02.000000 sparecores_runner-0.0.2/src/sparecores_runner.egg-info/top_level.txt
```

### Comparing `sparecores_runner-0.0.1/LICENSE` & `sparecores_runner-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sparecores_runner-0.0.1/pyproject.toml` & `sparecores_runner-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sparecores-runner"
-version = "0.0.1"
+version = "0.0.2"
 requires-python = ">= 3.9"
 dependencies = [
     "click",
     "pulumi",
     "pulumi-aws",
     "sparecores-crawler",
     "sparecores-data",
```

### Comparing `sparecores_runner-0.0.1/src/sc_runner/cli.py` & `sparecores_runner-0.0.2/src/sc_runner/cli.py`

 * *Files identical despite different names*

### Comparing `sparecores_runner-0.0.1/src/sc_runner/data.py` & `sparecores_runner-0.0.2/src/sc_runner/data.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-import sc_data
 from sc_crawler.tables import Server, ServerPrice, Datacenter, Vendor, Zone
 from sqlmodel import create_engine, Session, select
+import sc_data
 
 
 session = Session(create_engine(f"sqlite:///{sc_data.db.path}"))
 
 
 def vendors():
     return session.exec(select(Vendor.vendor_id)).all()
@@ -29,11 +29,11 @@
         stmt = stmt.where(ServerPrice.zone_id == zone)
     return [i[1] for i in session.exec(stmt.distinct()).all()]
 
 
 def servers_vendors(vendor: str, region: str | None = None, zone: str | None = None):
     stmt = select(ServerPrice.vendor_id, ServerPrice.datacenter_id, Zone.name, ServerPrice.server_id).join(Zone).where(ServerPrice.vendor_id == vendor)
     if region:
-        stmt = stmt.where(ServerPrice.datacenter_id==region)
+        stmt = stmt.where(ServerPrice.datacenter_id == region)
     if zone:
-        stmt = stmt.where(ServerPrice.zone_id==zone)
+        stmt = stmt.where(ServerPrice.zone_id == zone)
     return session.exec(stmt.distinct()).all()
```

### Comparing `sparecores_runner-0.0.1/src/sc_runner/resources/aws.py` & `sparecores_runner-0.0.2/src/sc_runner/resources/aws.py`

 * *Files identical despite different names*

### Comparing `sparecores_runner-0.0.1/src/sc_runner/resources/base.py` & `sparecores_runner-0.0.2/src/sc_runner/resources/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,9 +12,9 @@
     envvar, def_val = defaults[opt_name]
     return os.environ.get(envvar, json.dumps(def_val))
 
 
 def default(defaults, opt_name):
     """Return default value from `defaults` for the `opt_name` as a Python object(dict)."""
     envvar, def_val = defaults[opt_name]
-    return json.loads(os.environ.get(envvar, "null")) or defaults[opt_name]
+    return json.loads(os.environ.get(envvar, "null")) or def_val
```

### Comparing `sparecores_runner-0.0.1/src/sc_runner/runner.py` & `sparecores_runner-0.0.2/src/sc_runner/runner.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 def get_stack_name(vendor: str, func: Callable, resource_opts: dict) -> str:
     hints = get_type_hints(func, include_extras=True)
     stack_name = [vendor]
     for name, annotation in hints.items():
         for meta in getattr(annotation, "__metadata__", []):
             if isinstance(meta, resources.StackName):
-                stack_name.append(str(resource_opts[name]))
+                stack_name.append(str(resource_opts.get(name)))
     return ".".join(stack_name)
 
 
 def pulumi_stack(
     pulumi_program: Callable,
     project_name: Annotated[str, DefaultOpt(["--project-name"], type=str, help="Pulumi project name")] = os.environ.get("PULUMI_PROJECT_NAME", "runner"),
     work_dir: Annotated[str, DefaultOpt(["--work-dir"], type=str, help="Pulumi work dir")] = os.environ.get("PULUMI_WORK_DIR", "/data/workdir"),
```

