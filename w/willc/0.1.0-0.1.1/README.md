# Comparing `tmp/willc-0.1.0.tar.gz` & `tmp/willc-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "willc-0.1.0.tar", max compression
+gzip compressed data, was "willc-0.1.1.tar", max compression
```

## Comparing `willc-0.1.0.tar` & `willc-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1067 2024-04-23 23:51:19.131724 willc-0.1.0/LICENSE
--rw-r--r--   0        0        0     1974 2024-04-23 23:40:09.211353 willc-0.1.0/README.md
--rw-r--r--   0        0        0      551 2024-04-23 23:52:15.076830 willc-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-23 18:49:43.472317 willc-0.1.0/willc/__init__.py
--rw-r--r--   0        0        0     4431 2024-04-23 23:34:54.149557 willc-0.1.0/willc/main.py
--rw-r--r--   0        0        0     2756 1970-01-01 00:00:00.000000 willc-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-05-10 08:45:43.619376 willc-0.1.1/LICENSE
+-rw-r--r--   0        0        0     2031 2024-05-10 08:45:43.619590 willc-0.1.1/README.md
+-rw-r--r--   0        0        0      567 2024-05-10 10:39:37.016094 willc-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-10 09:19:54.870645 willc-0.1.1/willc/__init__.py
+-rw-r--r--   0        0        0     5964 2024-05-10 10:39:37.019174 willc-0.1.1/willc/main.py
+-rw-r--r--   0        0        0     2850 1970-01-01 00:00:00.000000 willc-0.1.1/PKG-INFO
```

### Comparing `willc-0.1.0/LICENSE` & `willc-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `willc-0.1.0/README.md` & `willc-0.1.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,29 @@
 ## willc
 
 My version of the `wc` tool, completing the first of John Crickett's [Coding Challenges](https://codingchallenges.fyi/challenges/challenge-wc)
 
+Install it with `pipx`:
+
+```
+pipx install willc
+```
+
 Here's a lightly adapted `man` page! (Since it's built with `typer`, you can just use the `--help` option, however!)
 
 **NAME**
+
 willc – word, line, character, and byte count
 
 **SYNOPSIS**
+
 `willc [-clmw] [file ...]`
 
 **DESCRIPTION**
+
 The willc utility displays the number of lines, words, and bytes contained in each input file, or standard input (if no file is specified) to the standard output.  A line is defined as a string of characters delimited by a ⟨newline⟩ character.  Characters beyond the final ⟨newline⟩ character will not be included in the line count.
 
 A word is defined as a string of characters delimited by white space characters.  White space characters are the set of characters for which the iswspace(3) function returns true.  If more than one input file is specified, a line of cumulative counts for all the files is displayed on a separate line after the output for the last file.
 
 The following options are available:
 
 `-c`: The number of bytes in each input file is written to the standard output.  This will cancel out any prior usage of the -m option.
@@ -23,8 +32,8 @@
 
 `-m`: The number of characters in each input file is written to the standard output.  If the current locale does not support multibyte characters, this is equivalent to the -c option.  This will cancel out any prior usage of the -c option.
 
 `-w`: The number of words in each input file is written to the standard output.
 
 When an option is specified, willc only reports the information requested by that option.  The order of output always takes the form of line, word, byte, and file name.  The default action is equivalent to specifying the -c, -l and -w options.
 
-If no files are specified, the standard input is used and no file name is displayed.
+If no files are specified, the standard input is used and no file name is displayed.
```

### Comparing `willc-0.1.0/pyproject.toml` & `willc-0.1.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 [tool.poetry]
 name = "willc"
-version = "0.1.0"
+version = "0.1.1"
 description = "My version of the `wc` tool"
 license = "MIT"
 authors = ["WillDenby <119456795+WillDenby@users.noreply.github.com>"]
 readme = "README.md"
 repository = "https://github.com/WillDenby/willc"
 
 [tool.poetry.scripts]
 willc = "willc.main:app"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 typer = "^0.12.3"
 pytest-mock = "^3.14.0"
 pytest-cov = "^5.0.0"
+ruff = "^0.4.4"
 
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^8.1.1"
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `willc-0.1.0/PKG-INFO` & `willc-0.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,41 +1,51 @@
 Metadata-Version: 2.1
 Name: willc
-Version: 0.1.0
+Version: 0.1.1
 Summary: My version of the `wc` tool
 Home-page: https://github.com/WillDenby/willc
 License: MIT
 Author: WillDenby
 Author-email: 119456795+WillDenby@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: pytest-cov (>=5.0.0,<6.0.0)
 Requires-Dist: pytest-mock (>=3.14.0,<4.0.0)
+Requires-Dist: ruff (>=0.4.4,<0.5.0)
 Requires-Dist: typer (>=0.12.3,<0.13.0)
 Project-URL: Repository, https://github.com/WillDenby/willc
 Description-Content-Type: text/markdown
 
 ## willc
 
 My version of the `wc` tool, completing the first of John Crickett's [Coding Challenges](https://codingchallenges.fyi/challenges/challenge-wc)
 
+Install it with `pipx`:
+
+```
+pipx install willc
+```
+
 Here's a lightly adapted `man` page! (Since it's built with `typer`, you can just use the `--help` option, however!)
 
 **NAME**
+
 willc – word, line, character, and byte count
 
 **SYNOPSIS**
+
 `willc [-clmw] [file ...]`
 
 **DESCRIPTION**
+
 The willc utility displays the number of lines, words, and bytes contained in each input file, or standard input (if no file is specified) to the standard output.  A line is defined as a string of characters delimited by a ⟨newline⟩ character.  Characters beyond the final ⟨newline⟩ character will not be included in the line count.
 
 A word is defined as a string of characters delimited by white space characters.  White space characters are the set of characters for which the iswspace(3) function returns true.  If more than one input file is specified, a line of cumulative counts for all the files is displayed on a separate line after the output for the last file.
 
 The following options are available:
 
 `-c`: The number of bytes in each input file is written to the standard output.  This will cancel out any prior usage of the -m option.
@@ -45,7 +55,8 @@
 `-m`: The number of characters in each input file is written to the standard output.  If the current locale does not support multibyte characters, this is equivalent to the -c option.  This will cancel out any prior usage of the -c option.
 
 `-w`: The number of words in each input file is written to the standard output.
 
 When an option is specified, willc only reports the information requested by that option.  The order of output always takes the form of line, word, byte, and file name.  The default action is equivalent to specifying the -c, -l and -w options.
 
 If no files are specified, the standard input is used and no file name is displayed.
+
```

