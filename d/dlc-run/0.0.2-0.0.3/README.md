# Comparing `tmp/dlc_run-0.0.2.tar.gz` & `tmp/dlc_run-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dlc_run-0.0.2.tar", last modified: Wed May  8 03:33:53 2024, max compression
+gzip compressed data, was "dist/dlc_run-0.0.3.tar", last modified: Fri May 10 09:27:26 2024, max compression
```

## Comparing `dlc_run-0.0.2.tar` & `dlc_run-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:33:53.000000 dlc_run-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-08 03:33:53.000000 dlc_run-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-08 03:33:49.000000 dlc_run-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:33:53.000000 dlc_run-0.0.2/dlc_run/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 03:33:49.000000 dlc_run-0.0.2/dlc_run/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7419 2024-05-08 03:33:49.000000 dlc_run-0.0.2/dlc_run/dlc_run.py
--rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-05-08 03:33:49.000000 dlc_run-0.0.2/dlc_run/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:33:53.000000 dlc_run-0.0.2/dlc_run.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-08 03:33:52.000000 dlc_run-0.0.2/dlc_run.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-08 03:33:53.000000 dlc_run-0.0.2/dlc_run.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 03:33:52.000000 dlc_run-0.0.2/dlc_run.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-08 03:33:52.000000 dlc_run-0.0.2/dlc_run.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-08 03:33:52.000000 dlc_run-0.0.2/dlc_run.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 03:33:53.000000 dlc_run-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4090 2024-05-08 03:33:49.000000 dlc_run-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:27:26.000000 dlc_run-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-10 09:27:26.000000 dlc_run-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-10 09:27:20.000000 dlc_run-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:27:26.000000 dlc_run-0.0.3/dlc_run/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 09:27:20.000000 dlc_run-0.0.3/dlc_run/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7374 2024-05-10 09:27:20.000000 dlc_run-0.0.3/dlc_run/dlc_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-05-10 09:27:20.000000 dlc_run-0.0.3/dlc_run/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:27:26.000000 dlc_run-0.0.3/dlc_run.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-10 09:27:26.000000 dlc_run-0.0.3/dlc_run.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-10 09:27:26.000000 dlc_run-0.0.3/dlc_run.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 09:27:26.000000 dlc_run-0.0.3/dlc_run.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-10 09:27:26.000000 dlc_run-0.0.3/dlc_run.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-10 09:27:26.000000 dlc_run-0.0.3/dlc_run.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 09:27:26.000000 dlc_run-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4090 2024-05-10 09:27:20.000000 dlc_run-0.0.3/setup.py
```

### Comparing `dlc_run-0.0.2/dlc_run/dlc_run.py` & `dlc_run-0.0.3/dlc_run/dlc_run.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,18 +9,19 @@
 
 def get_workspace_id(partition: str, config_path: str, dlc_path: str) -> str:
     """Extract the workspace ID for the specified partition using dlc
     command."""
     config_path = os.path.expanduser(config_path)
     dlc_path = os.path.expanduser(dlc_path)
     try:
-        result = subprocess.run([dlc_path, 'get', 'workspace', '-c', config_path],
-                                capture_output=True,
-                                text=True,
-                                check=True)
+        result = subprocess.run(
+            [dlc_path, 'get', 'workspace', '-c', config_path],
+            capture_output=True,
+            text=True,
+            check=True)
         regex = rf'\|\s*{re.escape(partition)}\s*\|\s*([\w]+)\s*\|'
         match = re.search(regex, result.stdout, re.MULTILINE)
         if match:
             return match.group(1).strip()
     except subprocess.SubprocessError as e:
         print(f'Error retrieving workspace ID: {e}')
         return None
@@ -57,15 +58,15 @@
 
 
 def parse_env_vars(env_vars):
     """Parse list of key=value strings into a dictionary, supporting both
     comma-separated and multiple inputs."""
     env_dict = {}
     for item in env_vars:
-        pairs = item.split(',')
+        pairs = item.split(';')
         for pair in pairs:
             if '=' in pair:
                 key, value = pair.split('=', 1)
                 env_dict[key.strip()] = value.strip()
     return env_dict
 
 
@@ -95,28 +96,28 @@
     parser.add_argument('--worker-count',
                         type=int,
                         default=1,
                         help='Number of workers')
     parser.add_argument('--worker-gpu',
                         type=int,
                         default=8,
-                        help='Total GPU count for the job')
+                        help='GPU count for single worker')
     parser.add_argument('--worker-cpu',
                         type=int,
                         default=120,
-                        help='Total CPU cores for the job')
+                        help='CPU count for single worker')
     parser.add_argument(
         '--worker-image',
         type=str,
         default='master0:5000/eflops/yehaochen:tears-and-blood1',
         help='Docker image for the worker')
     parser.add_argument('--worker-memory',
                         type=int,
                         default=800,
-                        help='Total memory in GB for the job')
+                        help='Memory in GB for single worker')
     parser.add_argument('--interactive',
                         action='store_true',
                         help='Whether to print out job status or not.')
     parser.add_argument('--shell',
                         type=str,
                         choices=['bash', 'zsh', 'none'],
                         default='none',
@@ -129,15 +130,15 @@
                         action='store_true',
                         help='Toggle proxy settings')
     parser.add_argument('--env',
                         '--environs',
                         action='append',
                         default=[],
                         help=('Additional environment variables, '
-                              "either `--env 'KEY1=VALUE1,KEY2=VALUE2'` or "
+                              "either `--env 'KEY1=VALUE1;KEY2=VALUE2'` or "
                               '`--env KEY1=VALUE1 --env KEY2=VALUE2`'))
 
     parser.add_argument(
         'task_cmds',
         # required=True,
         nargs=argparse.REMAINDER,
         help='Command line to execute, similar to typing in the shell.')
@@ -154,15 +155,15 @@
     conda_cmd = f'conda activate {args.conda_env}' if args.conda_env else ''
     if args.proxy:
         proxy_cmd = ('export http_proxy=http://58.34.83.134:31128 && '
                      'export https_proxy=http://58.34.83.134:31128')
     else:
         proxy_cmd = 'unset http_proxy;unset https_proxy'
     env_dict = parse_env_vars(args.env)
-    env_var_cmds = '; '.join(
+    env_var_cmds = ' && '.join(
         [f'export {key}={value}' for key, value in env_dict.items()])
 
     env_cmds = [
         cmd
         for cmd in [home_cmd, proxy_cmd, env_var_cmds, shell_cmd, conda_cmd]
         if cmd
     ]
```

### Comparing `dlc_run-0.0.2/dlc_run/version.py` & `dlc_run-0.0.3/dlc_run/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Copyright (c) OpenMMLab. All rights reserved.
-__version__ = '0.0.2'
+__version__ = '0.0.3'
 
 
 def parse_version_info(version_str: str, length: int = 4) -> tuple:
     """Parse a version string into a tuple.
 
     Args:
         version_str (str): The version string.
```

### Comparing `dlc_run-0.0.2/setup.py` & `dlc_run-0.0.3/setup.py`

 * *Files identical despite different names*

