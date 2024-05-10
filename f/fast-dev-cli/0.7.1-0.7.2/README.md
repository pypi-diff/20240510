# Comparing `tmp/fast_dev_cli-0.7.1.tar.gz` & `tmp/fast_dev_cli-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fast_dev_cli-0.7.1.tar", max compression
+gzip compressed data, was "fast_dev_cli-0.7.2.tar", max compression
```

## Comparing `fast_dev_cli-0.7.1.tar` & `fast_dev_cli-0.7.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1068 2024-03-06 06:08:37.265617 fast_dev_cli-0.7.1/LICENSE
--rw-r--r--   0        0        0     2109 2024-04-30 08:17:16.702283 fast_dev_cli-0.7.1/README.md
--rw-r--r--   0        0        0      392 2024-04-30 13:31:19.454648 fast_dev_cli-0.7.1/fast_dev_cli/__init__.py
--rw-r--r--   0        0        0       28 2024-03-06 06:08:37.266125 fast_dev_cli-0.7.1/fast_dev_cli/__main__.py
--rw-r--r--   0        0        0    20742 2024-04-30 13:35:34.884923 fast_dev_cli-0.7.1/fast_dev_cli/cli.py
--rw-r--r--   0        0        0        0 2024-03-06 06:08:37.266469 fast_dev_cli-0.7.1/fast_dev_cli/py.typed
--rw-r--r--   0        0        0     1407 2024-05-01 04:45:50.351656 fast_dev_cli-0.7.1/pyproject.toml
--rw-r--r--   0        0        0     3014 1970-01-01 00:00:00.000000 fast_dev_cli-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-03-06 06:08:37.265617 fast_dev_cli-0.7.2/LICENSE
+-rw-r--r--   0        0        0     2109 2024-04-30 08:17:16.702283 fast_dev_cli-0.7.2/README.md
+-rw-r--r--   0        0        0      392 2024-05-09 15:36:58.837450 fast_dev_cli-0.7.2/fast_dev_cli/__init__.py
+-rw-r--r--   0        0        0       28 2024-03-06 06:08:37.266125 fast_dev_cli-0.7.2/fast_dev_cli/__main__.py
+-rw-r--r--   0        0        0    21875 2024-05-09 15:38:31.432614 fast_dev_cli-0.7.2/fast_dev_cli/cli.py
+-rw-r--r--   0        0        0        0 2024-03-06 06:08:37.266469 fast_dev_cli-0.7.2/fast_dev_cli/py.typed
+-rw-r--r--   0        0        0     1407 2024-05-10 01:54:44.688753 fast_dev_cli-0.7.2/pyproject.toml
+-rw-r--r--   0        0        0     3014 1970-01-01 00:00:00.000000 fast_dev_cli-0.7.2/PKG-INFO
```

### Comparing `fast_dev_cli-0.7.1/LICENSE` & `fast_dev_cli-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fast_dev_cli-0.7.1/README.md` & `fast_dev_cli-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `fast_dev_cli-0.7.1/fast_dev_cli/cli.py` & `fast_dev_cli-0.7.2/fast_dev_cli/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,29 @@
+from __future__ import annotations
+
 import importlib.metadata
 import os
 import re
 import subprocess
 import sys
 from functools import cached_property
 from pathlib import Path
 from subprocess import CompletedProcess
-from typing import Type
+from typing import TYPE_CHECKING, Optional, Type
 
 if sys.version_info >= (3, 11):
     from enum import StrEnum
     from typing import Self
 else:  # pragma: no cover
     from strenum import StrEnum  # type:ignore[no-redef,assignment]
     from typing_extensions import Self
 
+if TYPE_CHECKING:
+    from typer.models import OptionInfo
+
 
 __version__ = importlib.metadata.version(Path(__file__).parent.name)
 
 
 def parse_files(args: list[str] | tuple[str, ...]) -> list[str]:
     return [i for i in args if not i.startswith("-")]
 
@@ -116,19 +121,25 @@
     cmd = ["poetry", "version", "-s"]
     if verbose:
         command = " ".join(cmd)
         echo(f"--> {command}")
     return capture_cmd_output(cmd)
 
 
+def _ensure_bool(value: bool | "OptionInfo") -> bool:
+    if not isinstance(value, bool):
+        value = getattr(value, "default", False)
+    return value
+
+
 def exit_if_run_failed(
     cmd: str, env=None, _exit=False, dry=False, **kw
 ) -> CompletedProcess:
     run_and_echo(cmd, dry=True)
-    if dry:
+    if _ensure_bool(dry):
         return CompletedProcess("", 0)
     if env is not None:
         env = {**os.environ, **env}
     r = _run_shell(cmd, env=env, **kw)
     if rc := r.returncode:
         if _exit:
             sys.exit(rc)
@@ -216,15 +227,15 @@
     part: BumpUp.PartChoices,
     commit: bool = Option(
         False, "--commit", "-c", help="Whether run `git commit` after version changed"
     ),
     dry: bool = Option(False, "--dry", help="Only print, not really run shell command"),
 ) -> None:
     """Bump up version string in pyproject.toml"""
-    return BumpUp(commit, part.value, dry=dry).run()
+    return BumpUp(_ensure_bool(commit), part.value, dry=dry).run()
 
 
 def bump() -> None:
     part, commit = "", False
     if args := sys.argv[2:]:
         if "-c" in args or "--commit" in args:
             commit = True
@@ -526,14 +537,16 @@
         paths = " ".join(self.args) if self.args else "."
         return self.to_cmd(paths, self.check_only)
 
 
 def lint(files=None, dry=False) -> None:
     if files is None:
         files = parse_files(sys.argv[1:])
+    if files and files[0] == "lint":
+        files = files[1:]
     LintCode(files, dry=dry).run()
 
 
 def check(files=None, dry=False) -> None:
     LintCode(files, check_only=True, _exit=True, dry=dry).run()
 
 
@@ -542,15 +555,15 @@
     files: list[str],
     check_only: bool = Option(False, "--check-only", "-c"),
     dry: bool = Option(False, "--dry", help="Only print, not really run shell command"),
 ) -> None:
     """Run: ruff check/format to reformat code and then mypy to check"""
     if isinstance(files, str):
         files = [files]
-    if check_only:
+    if _ensure_bool(check_only):
         check(files, dry=dry)
     else:
         lint(files, dry=dry)
 
 
 @cli.command(name="check")
 def only_check(
@@ -597,26 +610,28 @@
     Sync(filename, extras, save, dry=dry).run()
 
 
 def _should_run_test_script(path: Path) -> bool:
     return path.exists()
 
 
-@cli.command()
-def test(
+@cli.command(name="test")
+def coverage_test(
     dry: bool = Option(False, "--dry", help="Only print, not really run shell command"),
     ignore_script: bool = Option(False, "--ignore-script", "-i"),
 ) -> None:
     """Run unittest by pytest and report coverage"""
+    return test(dry, ignore_script)
+
+
+def test(dry: bool, ignore_script=False) -> None:
     cwd = Path.cwd()
     root = Project.get_work_dir(cwd=cwd, allow_cwd=True)
     test_script = root / "scripts" / "test.sh"
-    if not isinstance(ignore_script, bool):
-        ignore_script = getattr(ignore_script, "default", False)
-    if not ignore_script and _should_run_test_script(test_script):
+    if not _ensure_bool(ignore_script) and _should_run_test_script(test_script):
         cmd = f"sh {test_script.relative_to(root)}"
         if cwd != root:
             cmd = f"cd {root} && " + cmd
     else:
         cmd = 'coverage run -m pytest -s && coverage report --omit="tests/*" -m'
         if not is_venv() or not check_call("coverage --version"):
             sep = " && "
@@ -629,9 +644,33 @@
     dry: bool = Option(False, "--dry", help="Only print, not really run shell command"),
 ) -> None:
     """Shortcut for package publish"""
     cmd = "poetry publish --build"
     exit_if_run_failed(cmd, dry=dry)
 
 
+def dev(
+    port: int | None | "OptionInfo", host: str | None | "OptionInfo", dry=False
+) -> None:
+    cmd = "fastapi dev"
+    if (port := getattr(port, "default", port)) and port != 8000:
+        cmd += f" --port={port}"
+    if (host := getattr(host, "default", host)) and host not in (
+        "localhost",
+        "127.0.0.1",
+    ):
+        cmd += f" --host={host}"
+    exit_if_run_failed(cmd, dry=dry)
+
+
+@cli.command(name="dev")
+def runserver(
+    port: Optional[int] = Option(None, "-p", "--port"),
+    host: Optional[str] = Option(None, "-h", "--host"),
+    dry: bool = Option(False, "--dry", help="Only print, not really run shell command"),
+) -> None:
+    """Check code style without reformat"""
+    dev(port, host, dry=dry)
+
+
 if __name__ == "__main__":
     cli()  # pragma: no cover
```

### Comparing `fast_dev_cli-0.7.1/pyproject.toml` & `fast_dev_cli-0.7.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fast-dev-cli"
-version = "0.7.1"
+version = "0.7.2"
 description = ""
 authors = ["Waket Zheng <waketzheng@gmail.com>"]
 readme = "README.md"
 packages = [{include = "fast_dev_cli"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `fast_dev_cli-0.7.1/PKG-INFO` & `fast_dev_cli-0.7.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fast-dev-cli
-Version: 0.7.1
+Version: 0.7.2
 Summary: 
 Author: Waket Zheng
 Author-email: waketzheng@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: fast-dev-cli Version: 0.7.1 Summary: Author: Waket
+Metadata-Version: 2.1 Name: fast-dev-cli Version: 0.7.2 Summary: Author: Waket
 Zheng Author-email: waketzheng@gmail.com Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12 Provides-Extra: all
 Requires-Dist: bumpversion (>=0.6.0,<0.7.0) ; extra == "all" Requires-Dist:
 click (>=7.1.1) Requires-Dist: coverage (>=6.5.0) ; extra == "all" Requires-
 Dist: mypy (>=1.10.0,<2.0.0) ; extra == "all" Requires-Dist: pytest
```

