# Comparing `tmp/aws-butler-0.1.1.tar.gz` & `tmp/aws_butler-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws-butler-0.1.1.tar", last modified: Thu Jan 18 09:02:07 2024, max compression
+gzip compressed data, was "aws_butler-0.1.2.tar", last modified: Fri May 10 13:30:51 2024, max compression
```

## Comparing `aws-butler-0.1.1.tar` & `aws_butler-0.1.2.tar`

### file list

```diff
@@ -1,14 +1,16 @@
-drwxr-xr-x   0 alban     (1000) alban     (1000)        0 2024-01-18 09:02:07.774493 aws-butler-0.1.1/
--rw-r--r--   0 alban     (1000) alban     (1000)      216 2024-01-18 09:02:07.774493 aws-butler-0.1.1/PKG-INFO
--rw-r--r--   0 alban     (1000) alban     (1000)     2274 2024-01-17 16:03:15.000000 aws-butler-0.1.1/README.md
-drwxr-xr-x   0 alban     (1000) alban     (1000)        0 2024-01-18 09:02:07.774493 aws-butler-0.1.1/aws_butler.egg-info/
--rw-r--r--   0 alban     (1000) alban     (1000)      216 2024-01-18 09:02:07.000000 aws-butler-0.1.1/aws_butler.egg-info/PKG-INFO
--rw-r--r--   0 alban     (1000) alban     (1000)      262 2024-01-18 09:02:07.000000 aws-butler-0.1.1/aws_butler.egg-info/SOURCES.txt
--rw-r--r--   0 alban     (1000) alban     (1000)        1 2024-01-18 09:02:07.000000 aws-butler-0.1.1/aws_butler.egg-info/dependency_links.txt
--rw-r--r--   0 alban     (1000) alban     (1000)       76 2024-01-18 09:02:07.000000 aws-butler-0.1.1/aws_butler.egg-info/entry_points.txt
--rw-r--r--   0 alban     (1000) alban     (1000)       21 2024-01-18 09:02:07.000000 aws-butler-0.1.1/aws_butler.egg-info/requires.txt
--rw-r--r--   0 alban     (1000) alban     (1000)       22 2024-01-18 09:02:07.000000 aws-butler-0.1.1/aws_butler.egg-info/top_level.txt
--rw-r--r--   0 alban     (1000) alban     (1000)     6639 2024-01-16 13:51:50.000000 aws-butler-0.1.1/cloudwatch.py
--rw-r--r--   0 alban     (1000) alban     (1000)    11409 2024-01-18 09:00:05.000000 aws-butler-0.1.1/parameters.py
--rw-r--r--   0 alban     (1000) alban     (1000)      378 2024-01-18 09:02:07.774493 aws-butler-0.1.1/setup.cfg
--rw-r--r--   0 alban     (1000) alban     (1000)       73 2024-01-15 14:59:45.000000 aws-butler-0.1.1/setup.py
+drwxr-xr-x   0 alban     (1000) alban     (1000)        0 2024-05-10 13:30:51.853685 aws_butler-0.1.2/
+-rw-r--r--   0 alban     (1000) alban     (1000)      303 2024-05-10 13:30:51.853685 aws_butler-0.1.2/PKG-INFO
+-rw-r--r--   0 alban     (1000) alban     (1000)     2274 2024-01-17 16:03:15.000000 aws_butler-0.1.2/README.md
+drwxr-xr-x   0 alban     (1000) alban     (1000)        0 2024-05-10 13:30:51.843685 aws_butler-0.1.2/aws_butler.egg-info/
+-rw-r--r--   0 alban     (1000) alban     (1000)      303 2024-05-10 13:30:51.000000 aws_butler-0.1.2/aws_butler.egg-info/PKG-INFO
+-rw-r--r--   0 alban     (1000) alban     (1000)      287 2024-05-10 13:30:51.000000 aws_butler-0.1.2/aws_butler.egg-info/SOURCES.txt
+-rw-r--r--   0 alban     (1000) alban     (1000)        1 2024-05-10 13:30:51.000000 aws_butler-0.1.2/aws_butler.egg-info/dependency_links.txt
+-rw-r--r--   0 alban     (1000) alban     (1000)       76 2024-05-10 13:30:51.000000 aws_butler-0.1.2/aws_butler.egg-info/entry_points.txt
+-rw-r--r--   0 alban     (1000) alban     (1000)       49 2024-05-10 13:30:51.000000 aws_butler-0.1.2/aws_butler.egg-info/requires.txt
+-rw-r--r--   0 alban     (1000) alban     (1000)       22 2024-05-10 13:30:51.000000 aws_butler-0.1.2/aws_butler.egg-info/top_level.txt
+-rw-r--r--   0 alban     (1000) alban     (1000)     6639 2024-01-16 13:51:50.000000 aws_butler-0.1.2/cloudwatch.py
+-rw-r--r--   0 alban     (1000) alban     (1000)    11501 2024-05-10 13:18:56.000000 aws_butler-0.1.2/parameters.py
+-rw-r--r--   0 alban     (1000) alban     (1000)      434 2024-05-10 13:30:51.853685 aws_butler-0.1.2/setup.cfg
+-rw-r--r--   0 alban     (1000) alban     (1000)       73 2024-01-15 14:59:45.000000 aws_butler-0.1.2/setup.py
+drwxr-xr-x   0 alban     (1000) alban     (1000)        0 2024-05-10 13:30:51.843685 aws_butler-0.1.2/tests/
+-rw-r--r--   0 alban     (1000) alban     (1000)     1373 2024-05-10 13:23:05.000000 aws_butler-0.1.2/tests/test_parameters.py
```

### Comparing `aws-butler-0.1.1/README.md` & `aws_butler-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `aws-butler-0.1.1/cloudwatch.py` & `aws_butler-0.1.2/cloudwatch.py`

 * *Files identical despite different names*

### Comparing `aws-butler-0.1.1/parameters.py` & `aws_butler-0.1.2/parameters.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,38 +5,46 @@
 """
 
 import os
 import re
 import json
 import click
 import boto3
-from itertools import chain
+import botocore.client
+import dotenv
 from tabulate import tabulate
 from datetime import datetime
 from collections import namedtuple
 from concurrent.futures import ThreadPoolExecutor, as_completed
+from typing import Generator
 
 diff_summary = namedtuple("diff_summary", "unchanged new changed")
 change = namedtuple("change", "old new")
 
 
 def is_valid_ssm_name(name: str) -> tuple[bool, str]:
-    ALLOWED = "[a-zA-Z0-9_.-]"
+    allowed = "[a-zA-Z0-9_.-]"
+    arn_path = f"(?P<arn>arn:aws:ssm:\\w+-\\w+-\\d+:\\d+:parameter)?(?P<path>.+)"
+    if arn_path_match := re.match(arn_path, name):
+        arn, path = arn_path_match.groups()
+
     if len(name) > 1011:
         return False, "name cannot be longer than 1011 chars"
-    if name.count("/") > 14:
-        return False, "name cannot have more than 14 levels of hierachy"
-    if re.match("(?i)/?(aws)|(ssm)", name):
+    if name.count("/") > 15:
+        return False, "name cannot have more than 15 levels of hierachy"
+    if re.match("(?i)/?(aws)|(ssm)", path):
         return False, "name cannot start with 'aws' or 'ssm'"
-    if not re.match(f"^(/?(?=(?P<p1>{ALLOWED}+))(?P=p1))+$", name):
+    if not re.match(f"^(/|{allowed})+$", path):
         return False, "name uses an illegal character or pattern"
+    if not path.startswith("/") and "/" in path:
+        return False, "name must be fully qualified path"
     return True, "name is valid"
 
 
-def get_client(profile_name: str, resource_name: str) -> aws:
+def get_client(profile_name: str, resource_name: str) -> botocore.client.S3:
     session = boto3.Session(profile_name=profile_name)
     return session.client(resource_name)
 
 
 def epoch_to_str(unix_epoch: int, fmt: str | None = None) -> str:
     return datetime.fromtimestamp(unix_epoch).strftime(fmt or "%Y-%m-%d %H:%M:%S %z")
 
@@ -88,15 +96,15 @@
                 n_applied += 1
                 click.echo(f"successfully put parameter {future.result()}", err=True)
 
     return n_applied
 
 
 def walk_parameters(profile_name: str,
-                    path: tuple[str | None] | None = None,
+                    path: tuple[str | None, ...] | None = None,
                     limit: int | None=None,
                     *,
                     get_value: bool =False):
     """Generate parameters from parameter store, optionally filtered by a path
 
         The path can be full or partial, eg: '/path/to' or '/path/to/value'
     """
@@ -135,15 +143,15 @@
 
     for param in walk():
         if param["Name"] not in yielded_param_names:
             yield param
             yielded_param_names.add(param["Name"])
 
 
-def diff_params(local_params: dict[str: str], remote_params: dict[str: str]) -> diff_summary:
+def diff_params(local_params: dict[str, str], remote_params: dict[str, str]) -> diff_summary:
     unchanged = {}
     changed = {}
     new = {}
     for local_key, local_value in local_params.items():
         if local_key in remote_params:
             if local_value == remote_params[local_key]:
                 unchanged[local_key] = local_value
@@ -270,36 +278,26 @@
 @click.pass_context
 def push(ctx, env_file, path, dry_run):
     """Push parameters from a .env file to SSM
 
        All values will be stored as SecureString
     """
     local_params = {}
-
-    while line := env_file.readline():
-        line = line.strip()
-
-        if not line or line.startswith("#"):
-            continue
-
-        if "=" not in line:
-            raise ValueError(f"badly formatted .env file. expected '=' but not found on {line=}")
-
-        name, _, value = line.partition("=")
+    for name, value in dotenv.dotenv_values(stream=env_file).items():
         param_name = os.path.join(path, name.strip().lower())
 
         is_valid, message = is_valid_ssm_name(param_name)
         if not is_valid:
             raise ValueError(f"parameter {param_name!r} is not valid. {message}")
 
         local_params[param_name] = value.strip()
 
     remote_params = {
         param["Name"]: param["Value"]["Value"] for param in
-        walk_parameters(ctx.obj["profile"], path=local_params.keys(), get_value=True)
+        walk_parameters(ctx.obj["profile"], path=tuple(local_params.keys()), get_value=True)
     }
 
     diff = diff_params(local_params, remote_params)
 
     if dry_run:
         click.echo("No changes made")
         return
```

