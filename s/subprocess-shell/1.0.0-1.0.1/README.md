# Comparing `tmp/subprocess_shell-1.0.0.tar.gz` & `tmp/subprocess_shell-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "subprocess_shell-1.0.0.tar", last modified: Thu May  9 08:39:06 2024, max compression
+gzip compressed data, was "subprocess_shell-1.0.1.tar", last modified: Fri May 10 20:33:55 2024, max compression
```

## Comparing `subprocess_shell-1.0.0.tar` & `subprocess_shell-1.0.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 arappold  (1000) arappold  (1000)        0 2024-05-09 08:39:06.000000 subprocess_shell-1.0.0/
--rw-r--r--   0 arappold  (1000) arappold  (1000)     1072 2023-10-10 12:57:53.000000 subprocess_shell-1.0.0/LICENSE
--rw-r--r--   0 arappold  (1000) arappold  (1000)    20496 2024-05-09 08:39:06.000000 subprocess_shell-1.0.0/PKG-INFO
--rw-r--r--   0 arappold  (1000) arappold  (1000)    18616 2024-05-09 08:30:58.000000 subprocess_shell-1.0.0/README.md
--rw-r--r--   0 arappold  (1000) arappold  (1000)      583 2024-05-09 07:46:38.000000 subprocess_shell-1.0.0/pyproject.toml
--rw-r--r--   0 arappold  (1000) arappold  (1000)       38 2024-05-09 08:39:06.000000 subprocess_shell-1.0.0/setup.cfg
-drwxr-xr-x   0 arappold  (1000) arappold  (1000)        0 2024-05-09 08:39:06.000000 subprocess_shell-1.0.0/src/
-drwxr-xr-x   0 arappold  (1000) arappold  (1000)        0 2024-05-09 08:39:06.000000 subprocess_shell-1.0.0/src/subprocess_shell/
--rw-r--r--   0 arappold  (1000) arappold  (1000)    35431 2024-05-09 08:07:02.000000 subprocess_shell-1.0.0/src/subprocess_shell/__init__.py
-drwxr-xr-x   0 arappold  (1000) arappold  (1000)        0 2024-05-09 08:39:06.000000 subprocess_shell-1.0.0/src/subprocess_shell.egg-info/
--rw-r--r--   0 arappold  (1000) arappold  (1000)    20496 2024-05-09 08:39:06.000000 subprocess_shell-1.0.0/src/subprocess_shell.egg-info/PKG-INFO
--rw-r--r--   0 arappold  (1000) arappold  (1000)      315 2024-05-09 08:39:06.000000 subprocess_shell-1.0.0/src/subprocess_shell.egg-info/SOURCES.txt
--rw-r--r--   0 arappold  (1000) arappold  (1000)        1 2024-05-09 08:39:06.000000 subprocess_shell-1.0.0/src/subprocess_shell.egg-info/dependency_links.txt
--rw-r--r--   0 arappold  (1000) arappold  (1000)       62 2024-05-09 08:39:06.000000 subprocess_shell-1.0.0/src/subprocess_shell.egg-info/requires.txt
--rw-r--r--   0 arappold  (1000) arappold  (1000)       17 2024-05-09 08:39:06.000000 subprocess_shell-1.0.0/src/subprocess_shell.egg-info/top_level.txt
-drwxr-xr-x   0 arappold  (1000) arappold  (1000)        0 2024-05-09 08:39:06.000000 subprocess_shell-1.0.0/tests/
--rw-r--r--   0 arappold  (1000) arappold  (1000)    14509 2024-03-03 21:04:05.000000 subprocess_shell-1.0.0/tests/test_subprocess_shell.py
+drwxr-xr-x   0 arappold  (1000) arappold  (1000)        0 2024-05-10 20:33:55.000000 subprocess_shell-1.0.1/
+-rw-r--r--   0 arappold  (1000) arappold  (1000)     1072 2023-10-10 12:57:53.000000 subprocess_shell-1.0.1/LICENSE
+-rw-r--r--   0 arappold  (1000) arappold  (1000)    20496 2024-05-10 20:33:55.000000 subprocess_shell-1.0.1/PKG-INFO
+-rw-r--r--   0 arappold  (1000) arappold  (1000)    18616 2024-05-09 08:30:58.000000 subprocess_shell-1.0.1/README.md
+-rw-r--r--   0 arappold  (1000) arappold  (1000)      583 2024-05-10 20:29:36.000000 subprocess_shell-1.0.1/pyproject.toml
+-rw-r--r--   0 arappold  (1000) arappold  (1000)       38 2024-05-10 20:33:55.000000 subprocess_shell-1.0.1/setup.cfg
+drwxr-xr-x   0 arappold  (1000) arappold  (1000)        0 2024-05-10 20:33:55.000000 subprocess_shell-1.0.1/src/
+drwxr-xr-x   0 arappold  (1000) arappold  (1000)        0 2024-05-10 20:33:55.000000 subprocess_shell-1.0.1/src/subprocess_shell/
+-rw-r--r--   0 arappold  (1000) arappold  (1000)    35385 2024-05-10 20:15:10.000000 subprocess_shell-1.0.1/src/subprocess_shell/__init__.py
+drwxr-xr-x   0 arappold  (1000) arappold  (1000)        0 2024-05-10 20:33:55.000000 subprocess_shell-1.0.1/src/subprocess_shell.egg-info/
+-rw-r--r--   0 arappold  (1000) arappold  (1000)    20496 2024-05-10 20:33:55.000000 subprocess_shell-1.0.1/src/subprocess_shell.egg-info/PKG-INFO
+-rw-r--r--   0 arappold  (1000) arappold  (1000)      315 2024-05-10 20:33:55.000000 subprocess_shell-1.0.1/src/subprocess_shell.egg-info/SOURCES.txt
+-rw-r--r--   0 arappold  (1000) arappold  (1000)        1 2024-05-10 20:33:55.000000 subprocess_shell-1.0.1/src/subprocess_shell.egg-info/dependency_links.txt
+-rw-r--r--   0 arappold  (1000) arappold  (1000)       62 2024-05-10 20:33:55.000000 subprocess_shell-1.0.1/src/subprocess_shell.egg-info/requires.txt
+-rw-r--r--   0 arappold  (1000) arappold  (1000)       17 2024-05-10 20:33:55.000000 subprocess_shell-1.0.1/src/subprocess_shell.egg-info/top_level.txt
+drwxr-xr-x   0 arappold  (1000) arappold  (1000)        0 2024-05-10 20:33:55.000000 subprocess_shell-1.0.1/tests/
+-rw-r--r--   0 arappold  (1000) arappold  (1000)    16050 2024-05-10 20:23:03.000000 subprocess_shell-1.0.1/tests/test_subprocess_shell.py
```

### Comparing `subprocess_shell-1.0.0/LICENSE` & `subprocess_shell-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `subprocess_shell-1.0.0/PKG-INFO` & `subprocess_shell-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: subprocess_shell
-Version: 1.0.0
+Version: 1.0.1
 Summary: A shell for subprocess
 Author-email: Andreas Rappold <not_evil@rappold1.at>
 License: MIT License
         
         Copyright (c) 2023 Andreas Rappold
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `subprocess_shell-1.0.0/README.md` & `subprocess_shell-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `subprocess_shell-1.0.0/pyproject.toml` & `subprocess_shell-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "subprocess_shell"
-version = "1.0.0"
+version = "1.0.1"
 authors = [
   { name="Andreas Rappold", email="not_evil@rappold1.at" },
 ]
 description = "A shell for subprocess"
 readme = "README.md"
 
 [project.license]
```

### Comparing `subprocess_shell-1.0.0/src/subprocess_shell/__init__.py` & `subprocess_shell-1.0.1/src/subprocess_shell/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,19 +11,15 @@
 import subprocess
 import sys
 import threading
 import types
 import typing
 
 if typing.TYPE_CHECKING:
-    try:
-        import rich.style
-
-    except ImportError:
-        pass
+    import rich.style
 
 
 __all__ = ("start", "write", "wait", "read", "run")
 
 
 def _or(first_dictionary, second_dictionary):
     dictionary = dict(first_dictionary)
@@ -409,33 +405,37 @@
         else:
             previous_bytes = b""
             for bytes in itertools.chain([object], objects):
                 bytes = previous_bytes + bytes
                 try:
                     string = bytes.decode()
 
-                except UnicodeDecodeError as decode_error:
-                    for start_index in range(4):
-                        for stop_index in (None, -1, -2, -3):
-                            try:
-                                bytes[start_index:stop_index].decode()
+                except UnicodeDecodeError:
+                    for index in range(-3, 0):
+                        try:
+                            string = bytes[:index].decode()
 
-                            except UnicodeDecodeError:
-                                pass
+                        except UnicodeDecodeError:
+                            pass
 
-                            else:
-                                break
                         else:
-                            raise decode_error
+                            break
+                    else:
+                        if len(bytes) < 4:
+                            previous_bytes = bytes
+                            continue
+
+                        raise
 
-                    previous_bytes = bytes
+                    previous_bytes = bytes[index:]
 
                 else:
                     previous_bytes = b""
-                    yield string
+
+                yield string
 
             if previous_bytes != b"":
                 yield previous_bytes.decode()
 
     def get_stdout_bytes(self) -> typing.Generator[bytes, None, None]:
         """
         Yields chunks as bytes objects
```

### Comparing `subprocess_shell-1.0.0/src/subprocess_shell.egg-info/PKG-INFO` & `subprocess_shell-1.0.1/src/subprocess_shell.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: subprocess_shell
-Version: 1.0.0
+Version: 1.0.1
 Summary: A shell for subprocess
 Author-email: Andreas Rappold <not_evil@rappold1.at>
 License: MIT License
         
         Copyright (c) 2023 Andreas Rappold
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `subprocess_shell-1.0.0/tests/test_subprocess_shell.py` & `subprocess_shell-1.0.1/tests/test_subprocess_shell.py`

 * *Files 10% similar despite different names*

```diff
@@ -26,21 +26,25 @@
 I_ARGUMENTS = [sys.executable, "-c", _v_]
 
 I_STDOUT_PATTERN = lambda datetime_name, stdin_pattern, code_pattern=r"\d+": rf"""
 ╭─ (?P<_header>(?P<{datetime_name}>{DATETIME_PATTERN}) `{re.escape(subprocess.list2cmdline(I_ARGUMENTS))}`) (running|returned {code_pattern})
 │ stdout {stdin_pattern}
 ╰─ (?P=_header) returned {code_pattern}
 
-"""[1:-1]
+"""[
+    1:-1
+]
 I_STDERR_PATTERN = lambda datetime_name, stdin_pattern, code_pattern=r"\d+": rf"""
 ┏━ (?P<_header>(?P<{datetime_name}>{DATETIME_PATTERN}) `{re.escape(subprocess.list2cmdline(I_ARGUMENTS))}`) (running|returned {code_pattern})
 ┣ stderr {stdin_pattern}
 ┗━ (?P=_header) returned {code_pattern}
 
-"""[1:-1]
+"""[
+    1:-1
+]
 ECHO_ARGUMENTS = lambda string: (
     [sys.executable, "-c", f"print({repr(string)})"]
     if os.name == "nt"
     else ["echo", string]
 )
 CAT_ARGUMENTS = (
     [
@@ -156,97 +160,120 @@
 
     _v_ = dict(stdout=stdout_list.append, stderr=stderr_list.append)
     _test(lambda: I_ARGUMENTS, "", "", capsys, start=_v_, assert_=assert_)
 
 
 def test_1_fail(capsys):
     arguments = [sys.executable, "-c", "raise SystemExit(1)"]
-
     _test(lambda: arguments, "", "", capsys, wait=dict(return_codes=None), result=1)
-
-    _v_ = re.escape(subprocess.list2cmdline(arguments))
     _test(
         lambda: arguments,
         "",
         "",
         capsys,
         wait=dict(return_codes=(0,)),
         raises=subprocess_shell.ProcessFailedError,
-        raises_pattern=rf"^{DATETIME_PATTERN} `{_v_}` returned 1$",
+        raises_pattern=rf"^{DATETIME_PATTERN} `{re.escape(subprocess.list2cmdline(arguments))}` returned 1$",
     )
-
     _test(lambda: arguments, "", "", capsys, wait=dict(return_codes=(1,)), result=1)
 
 
 def test_2_trivial(capsys):
     _v_ = rf"""
 ╭─ (?P<_header>{DATETIME_PATTERN} `{re.escape(subprocess.list2cmdline(CAT_ARGUMENTS))}`) {CODE_PATTERN}
 │ this
 ╰─ (?P=_header) returned 0
 
-"""[1:-1]
+"""
+    _v_ = _v_[1:-1]
     _test(lambda: ECHO_ARGUMENTS("this") >> start() + CAT_ARGUMENTS, _v_, "", capsys)
 
 
 def test_2_wait(capsys):
     for stdout, stderr in itertools.product([False, True], [False, True]):
 
         def assert_(group_dictionary):
             _v_ = group_dictionary["d0"] != group_dictionary.get("d1")
             _v_ = _v_ and group_dictionary["d0"] != group_dictionary.get("d2")
             assert _v_ and not (
                 stdout and stderr and group_dictionary["d1"] != group_dictionary["d2"]
             )
 
+        _v_ = I_STDERR_PATTERN("d0", "") + (
+            rf"""
+┏━ (?P<_header2>(?P<d2>{DATETIME_PATTERN}) `{re.escape(subprocess.list2cmdline(I_ARGUMENTS))}`) {CODE_PATTERN}
+┣ stderr stdout 
+┣ 
+┗━ (?P=_header2) returned 0
+
+"""[
+                1:-1
+            ]
+            if stderr
+            else ""
+        )
         _test(
             lambda: I_ARGUMENTS >> start() + I_ARGUMENTS,
-            rf"""
+            (
+                rf"""
 ╭─ (?P<_header>(?P<d1>{DATETIME_PATTERN}) `{re.escape(subprocess.list2cmdline(I_ARGUMENTS))}`) {CODE_PATTERN}
 │ stdout stdout 
 │ 
 ╰─ (?P=_header) returned 0
 
-"""[1:-1] if stdout else "",
-            I_STDERR_PATTERN("d0", "") + (rf"""
-┏━ (?P<_header2>(?P<d2>{DATETIME_PATTERN}) `{re.escape(subprocess.list2cmdline(I_ARGUMENTS))}`) {CODE_PATTERN}
-┣ stderr stdout 
-┣ 
-┗━ (?P=_header2) returned 0
-
-"""[1:-1] if stderr else ""),
+"""[
+                    1:-1
+                ]
+                if stdout
+                else ""
+            ),
+            _v_,
             capsys,
             wait=dict(stdout=stdout, stderr=stderr),
             assert_=assert_,
         )
 
     for stdout, stderr in itertools.product([False, True], [False, True]):
 
         def assert_(group_dictionary):
             _v_ = group_dictionary["d0"] != group_dictionary.get("d1")
             _v_ = _v_ and group_dictionary["d0"] != group_dictionary.get("d2")
             assert _v_ and not (
                 stdout and stderr and group_dictionary["d1"] != group_dictionary["d2"]
             )
 
-        _test(
-            lambda: I_ARGUMENTS >> start() - I_ARGUMENTS,
-            I_STDOUT_PATTERN("d0", "") + (rf"""
+        _v_ = I_STDOUT_PATTERN("d0", "") + (
+            rf"""
 ╭─ (?P<_header2>(?P<d1>{DATETIME_PATTERN}) `{re.escape(subprocess.list2cmdline(I_ARGUMENTS))}`) {CODE_PATTERN}
 │ stdout stderr 
 │ 
 ╰─ (?P=_header2) returned 0
 
-"""[1:-1] if stdout else ""),
-            rf"""
+"""[
+                1:-1
+            ]
+            if stdout
+            else ""
+        )
+        _test(
+            lambda: I_ARGUMENTS >> start() - I_ARGUMENTS,
+            _v_,
+            (
+                rf"""
 ┏━ (?P<_header>(?P<d2>{DATETIME_PATTERN}) `{re.escape(subprocess.list2cmdline(I_ARGUMENTS))}`) {CODE_PATTERN}
 ┣ stderr stderr 
 ┣ 
 ┗━ (?P=_header) returned 0
 
-"""[1:-1] if stderr else "",
+"""[
+                    1:-1
+                ]
+                if stderr
+                else ""
+            ),
             capsys,
             wait=dict(stdout=stdout, stderr=stderr),
             assert_=assert_,
         )
 
 
 def test_2_fail():
@@ -321,18 +348,17 @@
 
     if expected_lines[-1] == "":
         expected_lines.pop()
 
     if os.name == "nt":
         expected_lines = [string.replace("\n", "\r\n") for string in expected_lines]
 
+    _v_ = os.name == "nt"
     _v_ = (
-        subprocess_shell._or(os.environ, {"PYTHONIOENCODING": "utf-8"})
-        if os.name == "nt"
-        else None
+        subprocess_shell._or(os.environ, {"PYTHONIOENCODING": "utf-8"}) if _v_ else None
     )
     _v_ = [sys.executable] >> start(bufsize=bufsize, env=_v_)
     process = _v_ >> write(
         f"""
 import sys
 
 for object in {repr(objects)}:
@@ -359,43 +385,92 @@
     arguments = ECHO_ARGUMENTS("[red]this[/red]")
 
     _v_ = rf"""
 ╭─ (?P<_header>{DATETIME_PATTERN} `{re.escape(subprocess.list2cmdline(arguments))}`) {CODE_PATTERN}
 │ \[red\]this\[/red\]
 ╰─ (?P=_header) returned 0
 
-"""[1:-1]
-    _test(lambda: arguments, _v_, "", capsys)
+"""
+    _test(lambda: arguments, _v_[1:-1], "", capsys)
 
 
 def test_ascii(capsys):
-    _v_ = "import sys; print('stdout'); print('stderr', file=sys.stderr)"
-    arguments = [sys.executable, "-c", _v_]
+    _v_ = sys.executable
+    _v_ = [_v_, "-c", "import sys; print('stdout'); print('stderr', file=sys.stderr)"]
+    arguments = _v_
 
-    _test(
-        lambda: arguments,
-        rf"""
+    _v_ = rf"""
 \+\- (?P<_header>{DATETIME_PATTERN} `{re.escape(subprocess.list2cmdline(arguments))}`) {CODE_PATTERN}
 \| stdout
 \| 
 \+\- (?P=_header) returned 0
 
-"""[1:-1],
+"""
+    _test(
+        lambda: arguments,
+        _v_[1:-1],
         rf"""
 EE (?P<_header>{DATETIME_PATTERN} `{re.escape(subprocess.list2cmdline(arguments))}`) {CODE_PATTERN}
 E stderr
 E 
 EE (?P=_header) returned 0
 
-"""[1:-1],
+"""[
+            1:-1
+        ],
         capsys,
         wait=dict(ascii=True),
     )
 
 
+_v_ = os.name == "nt" or subprocess_shell._FORCE_ASYNC
+
+
+@hypothesis.settings(
+    suppress_health_check=[hypothesis.HealthCheck.function_scoped_fixture],
+    print_blob=True,
+)
+@hypothesis.given(
+    string=h_strategies.text(),
+    length=h_strategies.integers(min_value=1, max_value=4),
+    bufsize=h_strategies.sampled_from([2, 3, 4, 5] if _v_ else [0, 2, 3, 4, 5]),
+)
+def test_unicode(string, length, bufsize, capsys):
+    bytes = string.encode()
+
+    _v_ = os.name == "nt"
+    _v_ = (
+        subprocess_shell._or(os.environ, {"PYTHONIOENCODING": "utf-8"}) if _v_ else None
+    )
+    _v_ = [sys.executable] >> start(bufsize=bufsize, env=_v_)
+    process = _v_ >> write(
+        f"""
+import sys
+
+bytes = {repr(bytes)}
+
+index = 0
+while True:
+    part_bytes = bytes[index : index + {repr(length)}]
+    if part_bytes == b"":
+        break
+
+    sys.stdout.buffer.write(part_bytes)
+    sys.stdout.flush()
+
+    index += {repr(length)}
+""",
+        close=True,
+    )
+
+    assert "".join(process.get_stdout_strings()) == string
+    assert process >> wait() == 0
+    _assert_std("", "", capsys)
+
+
 def _test(
     function,
     stdout_pattern,
     stderr_pattern,
     capsys,
     start=None,
     write=None,
```

