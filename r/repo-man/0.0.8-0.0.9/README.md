# Comparing `tmp/repo-man-0.0.8.tar.gz` & `tmp/repo_man-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "repo-man-0.0.8.tar", last modified: Mon Feb 12 18:32:02 2024, max compression
+gzip compressed data, was "repo_man-0.0.9.tar", last modified: Wed Apr 17 09:47:53 2024, max compression
```

## Comparing `repo-man-0.0.8.tar` & `repo_man-0.0.9.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 18:32:02.981075 repo-man-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-02-12 18:31:55.000000 repo-man-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-02-12 18:31:55.000000 repo-man-0.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-02-12 18:32:02.981075 repo-man-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-02-12 18:31:55.000000 repo-man-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-02-12 18:31:55.000000 repo-man-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     2687 2024-02-12 18:32:02.981075 repo-man-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-12 18:31:55.000000 repo-man-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 18:32:02.973075 repo-man-0.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 18:32:02.977075 repo-man-0.0.8/src/repo_man/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 18:31:55.000000 repo-man-0.0.8/src/repo_man/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-02-12 18:31:55.000000 repo-man-0.0.8/src/repo_man/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 18:32:02.977075 repo-man-0.0.8/src/repo_man/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 18:31:55.000000 repo-man-0.0.8/src/repo_man/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-02-12 18:31:55.000000 repo-man-0.0.8/src/repo_man/commands/add.py
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-02-12 18:31:55.000000 repo-man-0.0.8/src/repo_man/commands/edit.py
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-02-12 18:31:55.000000 repo-man-0.0.8/src/repo_man/commands/flavors.py
--rw-r--r--   0 runner    (1001) docker     (127)      449 2024-02-12 18:31:55.000000 repo-man-0.0.8/src/repo_man/commands/implode.py
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-02-12 18:31:55.000000 repo-man-0.0.8/src/repo_man/commands/init.py
--rw-r--r--   0 runner    (1001) docker     (127)      978 2024-02-12 18:31:55.000000 repo-man-0.0.8/src/repo_man/commands/list_repos.py
--rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-02-12 18:31:55.000000 repo-man-0.0.8/src/repo_man/commands/remove.py
--rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-02-12 18:31:55.000000 repo-man-0.0.8/src/repo_man/commands/sniff.py
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-02-12 18:31:55.000000 repo-man-0.0.8/src/repo_man/consts.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 18:31:55.000000 repo-man-0.0.8/src/repo_man/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-02-12 18:31:55.000000 repo-man-0.0.8/src/repo_man/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 18:32:02.981075 repo-man-0.0.8/src/repo_man.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-02-12 18:32:02.000000 repo-man-0.0.8/src/repo_man.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      858 2024-02-12 18:32:02.000000 repo-man-0.0.8/src/repo_man.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-12 18:32:02.000000 repo-man-0.0.8/src/repo_man.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-02-12 18:32:02.000000 repo-man-0.0.8/src/repo_man.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-02-12 18:32:02.000000 repo-man-0.0.8/src/repo_man.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-02-12 18:32:02.000000 repo-man-0.0.8/src/repo_man.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 18:32:02.981075 repo-man-0.0.8/test/
--rw-r--r--   0 runner    (1001) docker     (127)     4735 2024-02-12 18:31:55.000000 repo-man-0.0.8/test/test_add.py
--rw-r--r--   0 runner    (1001) docker     (127)      755 2024-02-12 18:31:55.000000 repo-man-0.0.8/test/test_edit.py
--rw-r--r--   0 runner    (1001) docker     (127)     2166 2024-02-12 18:31:55.000000 repo-man-0.0.8/test/test_flavors.py
--rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-02-12 18:31:55.000000 repo-man-0.0.8/test/test_implode.py
--rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-02-12 18:31:55.000000 repo-man-0.0.8/test/test_init.py
--rw-r--r--   0 runner    (1001) docker     (127)     3433 2024-02-12 18:31:55.000000 repo-man-0.0.8/test/test_list_repos.py
--rw-r--r--   0 runner    (1001) docker     (127)     2314 2024-02-12 18:31:55.000000 repo-man-0.0.8/test/test_remove.py
--rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-02-12 18:31:55.000000 repo-man-0.0.8/test/test_sniff.py
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-02-12 18:31:55.000000 repo-man-0.0.8/test/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:47:53.624982 repo_man-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-17 09:47:46.000000 repo_man-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-17 09:47:46.000000 repo_man-0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-04-17 09:47:53.624982 repo_man-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-17 09:47:46.000000 repo_man-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-17 09:47:46.000000 repo_man-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     2698 2024-04-17 09:47:53.624982 repo_man-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 09:47:46.000000 repo_man-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:47:53.616982 repo_man-0.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:47:53.620982 repo_man-0.0.9/src/repo_man/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 09:47:46.000000 repo_man-0.0.9/src/repo_man/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-04-17 09:47:46.000000 repo_man-0.0.9/src/repo_man/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:47:53.624982 repo_man-0.0.9/src/repo_man/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 09:47:46.000000 repo_man-0.0.9/src/repo_man/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-04-17 09:47:46.000000 repo_man-0.0.9/src/repo_man/commands/add.py
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-17 09:47:46.000000 repo_man-0.0.9/src/repo_man/commands/edit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-04-17 09:47:46.000000 repo_man-0.0.9/src/repo_man/commands/implode.py
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-17 09:47:46.000000 repo_man-0.0.9/src/repo_man/commands/init.py
+-rw-r--r--   0 runner    (1001) docker     (127)      937 2024-04-17 09:47:46.000000 repo_man-0.0.9/src/repo_man/commands/list_repos.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-04-17 09:47:46.000000 repo_man-0.0.9/src/repo_man/commands/remove.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-04-17 09:47:46.000000 repo_man-0.0.9/src/repo_man/commands/sniff.py
+-rw-r--r--   0 runner    (1001) docker     (127)      621 2024-04-17 09:47:46.000000 repo_man-0.0.9/src/repo_man/commands/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-17 09:47:46.000000 repo_man-0.0.9/src/repo_man/consts.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 09:47:46.000000 repo_man-0.0.9/src/repo_man/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-04-17 09:47:46.000000 repo_man-0.0.9/src/repo_man/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:47:53.624982 repo_man-0.0.9/src/repo_man.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-04-17 09:47:53.000000 repo_man-0.0.9/src/repo_man.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      854 2024-04-17 09:47:53.000000 repo_man-0.0.9/src/repo_man.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 09:47:53.000000 repo_man-0.0.9/src/repo_man.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-17 09:47:53.000000 repo_man-0.0.9/src/repo_man.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-17 09:47:53.000000 repo_man-0.0.9/src/repo_man.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-17 09:47:53.000000 repo_man-0.0.9/src/repo_man.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:47:53.624982 repo_man-0.0.9/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     4735 2024-04-17 09:47:46.000000 repo_man-0.0.9/test/test_add.py
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-04-17 09:47:46.000000 repo_man-0.0.9/test/test_edit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-04-17 09:47:46.000000 repo_man-0.0.9/test/test_implode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-04-17 09:47:46.000000 repo_man-0.0.9/test/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3433 2024-04-17 09:47:46.000000 repo_man-0.0.9/test/test_list_repos.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2314 2024-04-17 09:47:46.000000 repo_man-0.0.9/test/test_remove.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-04-17 09:47:46.000000 repo_man-0.0.9/test/test_sniff.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2146 2024-04-17 09:47:46.000000 repo_man-0.0.9/test/test_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-17 09:47:46.000000 repo_man-0.0.9/test/test_utils.py
```

### Comparing `repo-man-0.0.8/PKG-INFO` & `repo_man-0.0.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: repo-man
-Version: 0.0.8
-Summary: Manage repositories of different flavors.
+Version: 0.0.9
+Summary: Manage repositories of a variety of different types.
 Home-page: https://github.com/easy-as-python/repo-man
 Author: Dane Hillard
 Author-email: "Dane Hillard" <github@danehillard.com>
 License: MIT License
 Project-URL: Documentation, https://repo-man.readthedocs.org
 Project-URL: Source, https://github.com/easy-as-python/repo-man
 Project-URL: Tracker, https://github.com/easy-as-python/repo-man/issues
@@ -25,15 +25,15 @@
 Requires-Dist: furo; extra == "docs"
 Requires-Dist: myst-parser; extra == "docs"
 Requires-Dist: sphinx; extra == "docs"
 Requires-Dist: sphinx-autobuild; extra == "docs"
 
 # repo-man
 
-Manage repositories of different flavors.
+Manage repositories of a variety of different types.
 Read [the full documentation](https://repo-man.readthedocs.org) to learn more.
 
 ## Installation
 
 ```shell
 $ python -m pip install repo-man
 ```
```

### Comparing `repo-man-0.0.8/setup.cfg` & `repo_man-0.0.9/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [metadata]
 name = repo-man
-version = 0.0.8
-description = Manage repositories of different flavors.
+version = 0.0.9
+description = Manage repositories of a variety of different types.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/easy-as-python/repo-man
 author = Dane Hillard
 author_email = "Dane Hillard" <github@danehillard.com>
 license = MIT License
 license_files = LICENSE
```

### Comparing `repo-man-0.0.8/src/repo_man/cli.py` & `repo_man-0.0.9/src/repo_man/cli.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import configparser
 
 import click
 
 from repo_man.commands.add import add
 from repo_man.commands.edit import edit
-from repo_man.commands.flavors import flavors
 from repo_man.commands.implode import implode
 from repo_man.commands.init import init
 from repo_man.commands.list_repos import list_repos
 from repo_man.commands.remove import remove
 from repo_man.commands.sniff import sniff
+from repo_man.commands.types import types
 from repo_man.consts import REPO_TYPES_CFG
 
 
 @click.group(context_settings={"help_option_names": ["-h", "--help"]})
 @click.version_option(package_name="repo-man")
 @click.pass_context
 def cli(context: click.Context) -> None:  # pragma: no cover
@@ -23,14 +23,14 @@
     config.read(REPO_TYPES_CFG)
     context.obj = config
 
 
 def main() -> None:  # pragma: no cover
     cli.add_command(add)
     cli.add_command(edit)
-    cli.add_command(flavors)
+    cli.add_command(types)
     cli.add_command(implode)
     cli.add_command(init)
     cli.add_command(list_repos)
     cli.add_command(remove)
     cli.add_command(sniff)
     cli()
```

### Comparing `repo-man-0.0.8/src/repo_man/commands/add.py` & `repo_man-0.0.9/src/repo_man/commands/add.py`

 * *Files identical despite different names*

### Comparing `repo-man-0.0.8/src/repo_man/commands/flavors.py` & `repo_man-0.0.9/src/repo_man/commands/types.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from repo_man.utils import ensure_config_file_exists, pass_config
 
 
 @click.command
 @click.argument("repo", type=click.Path(exists=True, file_okay=False))
 @pass_config
-def flavors(config: configparser.ConfigParser, repo: str) -> None:
+def types(config: configparser.ConfigParser, repo: str) -> None:
     """List the configured types for a repository"""
 
     ensure_config_file_exists()
 
     found = set()
 
     for section in config.sections():
```

### Comparing `repo-man-0.0.8/src/repo_man/commands/init.py` & `repo_man-0.0.9/src/repo_man/commands/init.py`

 * *Files identical despite different names*

### Comparing `repo-man-0.0.8/src/repo_man/commands/list_repos.py` & `repo_man-0.0.9/src/repo_man/commands/list_repos.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import configparser
 
 import click
 
 from repo_man.utils import ensure_config_file_exists, parse_repo_types, pass_config
 
 
-@click.command(name="list", help="The type of repository to manage")
+@click.command(name="list")
 @click.option("-t", "--type", "repo_types", multiple=True, show_choices=False, required=True)
 @pass_config
 def list_repos(config: configparser.ConfigParser, repo_types: list[str]) -> None:
     """List matching repositories"""
 
     ensure_config_file_exists()
```

### Comparing `repo-man-0.0.8/src/repo_man/commands/remove.py` & `repo_man-0.0.9/src/repo_man/commands/remove.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import click
 
 from repo_man.consts import REPO_TYPES_CFG
 from repo_man.utils import ensure_config_file_exists, parse_repo_types, pass_config
 
 
-@click.command(name="remove", help="Remove a repository from one or more types")
+@click.command(name="remove")
 @click.option("-t", "--type", "repo_types", multiple=True, help="The types from which to remove the repository")
 @click.argument("repo", type=click.Path(exists=True, file_okay=False))
 @pass_config
 def remove(config: configparser.ConfigParser, repo: str, repo_types: list[str]) -> None:
     """Remove a repository from some or all types"""
 
     ensure_config_file_exists()
```

### Comparing `repo-man-0.0.8/src/repo_man/commands/sniff.py` & `repo_man-0.0.9/src/repo_man/commands/sniff.py`

 * *Files identical despite different names*

### Comparing `repo-man-0.0.8/src/repo_man/utils.py` & `repo_man-0.0.9/src/repo_man/utils.py`

 * *Files identical despite different names*

### Comparing `repo-man-0.0.8/src/repo_man.egg-info/PKG-INFO` & `repo_man-0.0.9/src/repo_man.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: repo-man
-Version: 0.0.8
-Summary: Manage repositories of different flavors.
+Version: 0.0.9
+Summary: Manage repositories of a variety of different types.
 Home-page: https://github.com/easy-as-python/repo-man
 Author: Dane Hillard
 Author-email: "Dane Hillard" <github@danehillard.com>
 License: MIT License
 Project-URL: Documentation, https://repo-man.readthedocs.org
 Project-URL: Source, https://github.com/easy-as-python/repo-man
 Project-URL: Tracker, https://github.com/easy-as-python/repo-man/issues
@@ -25,15 +25,15 @@
 Requires-Dist: furo; extra == "docs"
 Requires-Dist: myst-parser; extra == "docs"
 Requires-Dist: sphinx; extra == "docs"
 Requires-Dist: sphinx-autobuild; extra == "docs"
 
 # repo-man
 
-Manage repositories of different flavors.
+Manage repositories of a variety of different types.
 Read [the full documentation](https://repo-man.readthedocs.org) to learn more.
 
 ## Installation
 
 ```shell
 $ python -m pip install repo-man
 ```
```

### Comparing `repo-man-0.0.8/src/repo_man.egg-info/SOURCES.txt` & `repo_man-0.0.9/src/repo_man.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -14,22 +14,22 @@
 src/repo_man.egg-info/dependency_links.txt
 src/repo_man.egg-info/entry_points.txt
 src/repo_man.egg-info/requires.txt
 src/repo_man.egg-info/top_level.txt
 src/repo_man/commands/__init__.py
 src/repo_man/commands/add.py
 src/repo_man/commands/edit.py
-src/repo_man/commands/flavors.py
 src/repo_man/commands/implode.py
 src/repo_man/commands/init.py
 src/repo_man/commands/list_repos.py
 src/repo_man/commands/remove.py
 src/repo_man/commands/sniff.py
+src/repo_man/commands/types.py
 test/test_add.py
 test/test_edit.py
-test/test_flavors.py
 test/test_implode.py
 test/test_init.py
 test/test_list_repos.py
 test/test_remove.py
 test/test_sniff.py
+test/test_types.py
 test/test_utils.py
```

### Comparing `repo-man-0.0.8/test/test_add.py` & `repo_man-0.0.9/test/test_add.py`

 * *Files identical despite different names*

### Comparing `repo-man-0.0.8/test/test_edit.py` & `repo_man-0.0.9/test/test_edit.py`

 * *Files identical despite different names*

### Comparing `repo-man-0.0.8/test/test_flavors.py` & `repo_man-0.0.9/test/test_types.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 import configparser
 from pathlib import Path
 from typing import Callable
 
 import click
 
-from repo_man.commands.flavors import flavors
+from repo_man.commands.types import types
 
 
-def test_flavors_clean(runner: click.testing.CliRunner, get_config: Callable[[], configparser.ConfigParser]) -> None:
+def test_types_clean(runner: click.testing.CliRunner, get_config: Callable[[], configparser.ConfigParser]) -> None:
     with runner.isolated_filesystem():
         Path("some-repo").mkdir()
         config = get_config()
-        result = runner.invoke(flavors, ["some-repo"], obj=config)
+        result = runner.invoke(types, ["some-repo"], obj=config)
         assert result.exit_code == 1
         assert result.output == "No repo-man.cfg file found.\n"
 
 
-def test_flavors_when_configured(
+def test_types_when_configured(
     runner: click.testing.CliRunner, get_config: Callable[[], configparser.ConfigParser]
 ) -> None:
     with runner.isolated_filesystem():
         Path("some-repo").mkdir()
 
         with open("repo-man.cfg", "w") as config_file:
             config_file.write(
@@ -32,20 +32,20 @@
 known = 
 	some-other-repo
 
 """
             )
 
         config = get_config()
-        result = runner.invoke(flavors, ["some-repo"], obj=config)
+        result = runner.invoke(types, ["some-repo"], obj=config)
         assert result.exit_code == 0
         assert result.output == "foo\n"
 
 
-def test_flavors_when_not_configured(
+def test_types_when_not_configured(
     runner: click.testing.CliRunner, get_config: Callable[[], configparser.ConfigParser]
 ) -> None:
     with runner.isolated_filesystem():
         Path("some-repo").mkdir()
 
         with open("repo-man.cfg", "w") as config_file:
             config_file.write(
@@ -53,20 +53,20 @@
 known = 
 	some-other-repo
 
 """
             )
 
         config = get_config()
-        result = runner.invoke(flavors, ["some-repo"], obj=config)
+        result = runner.invoke(types, ["some-repo"], obj=config)
         assert result.exit_code == 0
         assert result.output == ""
 
 
-def test_flavors_when_ignored(
+def test_types_when_ignored(
     runner: click.testing.CliRunner, get_config: Callable[[], configparser.ConfigParser]
 ) -> None:
     with runner.isolated_filesystem():
         Path("some-repo").mkdir()
 
         with open("repo-man.cfg", "w") as config_file:
             config_file.write(
@@ -74,10 +74,10 @@
 known = 
 	some-repo
 
 """
             )
 
         config = get_config()
-        result = runner.invoke(flavors, ["some-repo"], obj=config)
+        result = runner.invoke(types, ["some-repo"], obj=config)
         assert result.exit_code == 0
         assert result.output == ""
```

### Comparing `repo-man-0.0.8/test/test_implode.py` & `repo_man-0.0.9/test/test_implode.py`

 * *Files identical despite different names*

### Comparing `repo-man-0.0.8/test/test_init.py` & `repo_man-0.0.9/test/test_init.py`

 * *Files identical despite different names*

### Comparing `repo-man-0.0.8/test/test_list_repos.py` & `repo_man-0.0.9/test/test_list_repos.py`

 * *Files identical despite different names*

### Comparing `repo-man-0.0.8/test/test_remove.py` & `repo_man-0.0.9/test/test_remove.py`

 * *Files identical despite different names*

### Comparing `repo-man-0.0.8/test/test_sniff.py` & `repo_man-0.0.9/test/test_sniff.py`

 * *Files identical despite different names*

