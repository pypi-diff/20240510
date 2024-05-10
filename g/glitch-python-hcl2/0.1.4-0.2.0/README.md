# Comparing `tmp/glitch-python-hcl2-0.1.4.tar.gz` & `tmp/glitch-python-hcl2-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glitch-python-hcl2-0.1.4.tar", last modified: Thu Mar  2 17:32:49 2023, max compression
+gzip compressed data, was "glitch-python-hcl2-0.2.0.tar", last modified: Fri May 10 11:32:28 2024, max compression
```

## Comparing `glitch-python-hcl2-0.1.4.tar` & `glitch-python-hcl2-0.2.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 joaogoncalves   (501) staff       (20)        0 2023-03-02 17:32:49.622942 glitch-python-hcl2-0.1.4/
--rw-r--r--   0 joaogoncalves   (501) staff       (20)     4286 2023-02-27 17:16:16.000000 glitch-python-hcl2-0.1.4/CHANGELOG.md
--rw-r--r--   0 joaogoncalves   (501) staff       (20)     1063 2023-02-27 17:16:16.000000 glitch-python-hcl2-0.1.4/LICENSE
--rw-r--r--   0 joaogoncalves   (501) staff       (20)      141 2023-02-27 17:16:16.000000 glitch-python-hcl2-0.1.4/MANIFEST.in
--rw-r--r--   0 joaogoncalves   (501) staff       (20)     3819 2023-03-02 17:32:49.622214 glitch-python-hcl2-0.1.4/PKG-INFO
--rw-r--r--   0 joaogoncalves   (501) staff       (20)     2935 2023-02-27 18:59:52.000000 glitch-python-hcl2-0.1.4/README.md
-drwxr-xr-x   0 joaogoncalves   (501) staff       (20)        0 2023-03-02 17:32:49.433094 glitch-python-hcl2-0.1.4/glitch_python_hcl2.egg-info/
--rw-r--r--   0 joaogoncalves   (501) staff       (20)     3819 2023-03-02 17:32:48.000000 glitch-python-hcl2-0.1.4/glitch_python_hcl2.egg-info/PKG-INFO
--rw-r--r--   0 joaogoncalves   (501) staff       (20)      370 2023-03-02 17:32:48.000000 glitch-python-hcl2-0.1.4/glitch_python_hcl2.egg-info/SOURCES.txt
--rw-r--r--   0 joaogoncalves   (501) staff       (20)        1 2023-03-02 17:32:48.000000 glitch-python-hcl2-0.1.4/glitch_python_hcl2.egg-info/dependency_links.txt
--rw-r--r--   0 joaogoncalves   (501) staff       (20)       17 2023-03-02 17:32:48.000000 glitch-python-hcl2-0.1.4/glitch_python_hcl2.egg-info/requires.txt
--rw-r--r--   0 joaogoncalves   (501) staff       (20)       10 2023-03-02 17:32:48.000000 glitch-python-hcl2-0.1.4/glitch_python_hcl2.egg-info/top_level.txt
-drwxr-xr-x   0 joaogoncalves   (501) staff       (20)        0 2023-03-02 17:32:49.621347 glitch-python-hcl2-0.1.4/hcl2/
--rw-r--r--   0 joaogoncalves   (501) staff       (20)      176 2023-02-27 17:16:16.000000 glitch-python-hcl2-0.1.4/hcl2/__init__.py
--rw-r--r--   0 joaogoncalves   (501) staff       (20)     3905 2023-02-27 17:16:16.000000 glitch-python-hcl2-0.1.4/hcl2/__main__.py
--rw-r--r--   0 joaogoncalves   (501) staff       (20)     1173 2023-02-27 17:16:16.000000 glitch-python-hcl2-0.1.4/hcl2/api.py
--rw-r--r--   0 joaogoncalves   (501) staff       (20)     3408 2023-02-27 17:43:41.000000 glitch-python-hcl2-0.1.4/hcl2/hcl2.lark
--rw-r--r--   0 joaogoncalves   (501) staff       (20)      378 2023-02-27 17:16:16.000000 glitch-python-hcl2-0.1.4/hcl2/parser.py
--rw-r--r--   0 joaogoncalves   (501) staff       (20)        0 2023-02-27 17:16:16.000000 glitch-python-hcl2-0.1.4/hcl2/py.typed
--rw-r--r--   0 joaogoncalves   (501) staff       (20)    14151 2023-03-02 17:31:20.000000 glitch-python-hcl2-0.1.4/hcl2/transformer.py
--rw-r--r--   0 joaogoncalves   (501) staff       (20)       38 2023-03-02 17:32:49.623078 glitch-python-hcl2-0.1.4/setup.cfg
--rw-r--r--   0 joaogoncalves   (501) staff       (20)     1652 2023-03-02 17:31:37.000000 glitch-python-hcl2-0.1.4/setup.py
+drwxrwxr-x   0 nfsaavedra  (1000) nfsaavedra  (1000)        0 2024-05-10 11:32:28.750474 glitch-python-hcl2-0.2.0/
+-rw-rw-r--   0 nfsaavedra  (1000) nfsaavedra  (1000)     4902 2024-05-09 16:10:12.000000 glitch-python-hcl2-0.2.0/CHANGELOG.md
+-rw-rw-r--   0 nfsaavedra  (1000) nfsaavedra  (1000)     1063 2024-05-09 16:08:34.000000 glitch-python-hcl2-0.2.0/LICENSE
+-rw-rw-r--   0 nfsaavedra  (1000) nfsaavedra  (1000)      141 2024-05-09 16:08:34.000000 glitch-python-hcl2-0.2.0/MANIFEST.in
+-rw-rw-r--   0 nfsaavedra  (1000) nfsaavedra  (1000)     4215 2024-05-10 11:32:28.750474 glitch-python-hcl2-0.2.0/PKG-INFO
+-rw-rw-r--   0 nfsaavedra  (1000) nfsaavedra  (1000)     3311 2024-05-09 16:11:03.000000 glitch-python-hcl2-0.2.0/README.md
+drwxrwxr-x   0 nfsaavedra  (1000) nfsaavedra  (1000)        0 2024-05-10 11:32:28.750474 glitch-python-hcl2-0.2.0/glitch_python_hcl2.egg-info/
+-rw-r--r--   0 nfsaavedra  (1000) nfsaavedra  (1000)     4215 2024-05-10 11:32:28.000000 glitch-python-hcl2-0.2.0/glitch_python_hcl2.egg-info/PKG-INFO
+-rw-rw-r--   0 nfsaavedra  (1000) nfsaavedra  (1000)      370 2024-05-10 11:32:28.000000 glitch-python-hcl2-0.2.0/glitch_python_hcl2.egg-info/SOURCES.txt
+-rw-rw-r--   0 nfsaavedra  (1000) nfsaavedra  (1000)        1 2024-05-10 11:32:28.000000 glitch-python-hcl2-0.2.0/glitch_python_hcl2.egg-info/dependency_links.txt
+-rw-rw-r--   0 nfsaavedra  (1000) nfsaavedra  (1000)       17 2024-05-10 11:32:28.000000 glitch-python-hcl2-0.2.0/glitch_python_hcl2.egg-info/requires.txt
+-rw-rw-r--   0 nfsaavedra  (1000) nfsaavedra  (1000)       10 2024-05-10 11:32:28.000000 glitch-python-hcl2-0.2.0/glitch_python_hcl2.egg-info/top_level.txt
+drwxrwxr-x   0 nfsaavedra  (1000) nfsaavedra  (1000)        0 2024-05-10 11:32:28.750474 glitch-python-hcl2-0.2.0/hcl2/
+-rw-rw-r--   0 nfsaavedra  (1000) nfsaavedra  (1000)      176 2024-05-09 16:08:34.000000 glitch-python-hcl2-0.2.0/hcl2/__init__.py
+-rw-rw-r--   0 nfsaavedra  (1000) nfsaavedra  (1000)     3905 2024-05-09 16:08:34.000000 glitch-python-hcl2-0.2.0/hcl2/__main__.py
+-rw-rw-r--   0 nfsaavedra  (1000) nfsaavedra  (1000)     1173 2024-05-09 16:08:34.000000 glitch-python-hcl2-0.2.0/hcl2/api.py
+-rw-rw-r--   0 nfsaavedra  (1000) nfsaavedra  (1000)     3450 2024-05-09 16:10:12.000000 glitch-python-hcl2-0.2.0/hcl2/hcl2.lark
+-rw-rw-r--   0 nfsaavedra  (1000) nfsaavedra  (1000)      378 2024-05-09 16:08:34.000000 glitch-python-hcl2-0.2.0/hcl2/parser.py
+-rw-rw-r--   0 nfsaavedra  (1000) nfsaavedra  (1000)        0 2024-05-09 16:08:34.000000 glitch-python-hcl2-0.2.0/hcl2/py.typed
+-rw-rw-r--   0 nfsaavedra  (1000) nfsaavedra  (1000)    14911 2024-05-10 10:39:04.000000 glitch-python-hcl2-0.2.0/hcl2/transformer.py
+-rw-rw-r--   0 nfsaavedra  (1000) nfsaavedra  (1000)       38 2024-05-10 11:32:28.750474 glitch-python-hcl2-0.2.0/setup.cfg
+-rw-rw-r--   0 nfsaavedra  (1000) nfsaavedra  (1000)     1701 2024-05-10 11:32:15.000000 glitch-python-hcl2-0.2.0/setup.py
```

### Comparing `glitch-python-hcl2-0.1.4/CHANGELOG.md` & `glitch-python-hcl2-0.2.0/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,33 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/)
 and this project adheres to [Semantic Versioning](http://semver.org/spec/v2.0.0.html).
 
+## \[4.3.3\] - 2024-03-27
+
+### Added
+
+- Support for Python 3.12 ([#153](https://github.com/amplify-education/python-hcl2/pull/153))
+
+## \[4.3.2\] - 2023-05-24
+
+### Added
+
+- Support for the conditional inside the nested locals without parentheses ([#138](https://github.com/amplify-education/python-hcl2/pull/129))
+
+## \[4.3.1\] - 2023-05-02
+
+### Added
+
+- Support for the braces in the next line. Thanks @rout39574 ([#129](https://github.com/amplify-education/python-hcl2/pull/129))
+- Support for the ternary multi-line expression. Thanks @seksham ([#128](https://github.com/amplify-education/python-hcl2/pull/128))
+
 ## \[4.3.0\] - 2022-01-16
 
 ### Added
 
 - Add tests for multiline comments inside a tuple ([#118](https://github.com/amplify-education/python-hcl2/pull/118))
 - Add `__begin_line__` and `__end_line__` meta parameters ([#120](https://github.com/amplify-education/python-hcl2/pull/120))
 - Add feature to parse comments in function args and list elems ([#119](https://github.com/amplify-education/python-hcl2/pull/119))
```

### Comparing `glitch-python-hcl2-0.1.4/LICENSE` & `glitch-python-hcl2-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `glitch-python-hcl2-0.1.4/PKG-INFO` & `glitch-python-hcl2-0.2.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: glitch-python-hcl2
-Version: 0.1.4
+Version: 0.2.0
 Summary: A parser for HCL2
 Home-page: https://github.com/joaotgoncalves/python-hcl2
 Author: João Gonçalves
 Author-email: joao.marques.goncalves@tecnico.ulisboa.pt
 License: MIT
+Platform: UNKNOWN
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
@@ -17,14 +18,16 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+[![Codacy Badge](https://app.codacy.com/project/badge/Grade/2e2015f9297346cbaa788c46ab957827)](https://app.codacy.com/gh/amplify-education/python-hcl2/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_grade)
+[![Build Status](https://travis-ci.org/amplify-education/python-hcl2.svg?branch=master)](https://travis-ci.org/amplify-education/python-hcl2)
 [![License](https://img.shields.io/badge/license-MIT-blue.svg)](https://raw.githubusercontent.com/amplify-education/python-hcl2/master/LICENSE)
 
 # Notice
 
 This is a fork of Amplify's [Python HCL2](https://github.com/amplify-education/python-hcl2) repository. This repository went through minor changes to work better with [GLITCH](https://github.com/sr-lab/GLITCH) and as the changes concern only the structure representation to be compatible with [GLITCH](https://github.com/sr-lab/GLITCH) we decided not to request updates for the upstream project. The two projects diverge in the representation of some structures and pushing new changes upstream doesn't make sense.
 
 # Python HCL2
@@ -94,7 +97,9 @@
 
 We welcome pull requests! For your pull request to be accepted smoothly, we suggest that you:
 
 - For any sizable change, first open a GitHub issue to discuss your idea.
 - Create a pull request.  Explain why you want to make the change and what it’s for.
 
 We’ll try to answer any PR’s promptly.
+
+
```

### Comparing `glitch-python-hcl2-0.1.4/README.md` & `glitch-python-hcl2-0.2.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+[![Codacy Badge](https://app.codacy.com/project/badge/Grade/2e2015f9297346cbaa788c46ab957827)](https://app.codacy.com/gh/amplify-education/python-hcl2/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_grade)
+[![Build Status](https://travis-ci.org/amplify-education/python-hcl2.svg?branch=master)](https://travis-ci.org/amplify-education/python-hcl2)
 [![License](https://img.shields.io/badge/license-MIT-blue.svg)](https://raw.githubusercontent.com/amplify-education/python-hcl2/master/LICENSE)
 
 # Notice
 
 This is a fork of Amplify's [Python HCL2](https://github.com/amplify-education/python-hcl2) repository. This repository went through minor changes to work better with [GLITCH](https://github.com/sr-lab/GLITCH) and as the changes concern only the structure representation to be compatible with [GLITCH](https://github.com/sr-lab/GLITCH) we decided not to request updates for the upstream project. The two projects diverge in the representation of some structures and pushing new changes upstream doesn't make sense.
 
 # Python HCL2
```

### Comparing `glitch-python-hcl2-0.1.4/glitch_python_hcl2.egg-info/PKG-INFO` & `glitch-python-hcl2-0.2.0/glitch_python_hcl2.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: glitch-python-hcl2
-Version: 0.1.4
+Version: 0.2.0
 Summary: A parser for HCL2
 Home-page: https://github.com/joaotgoncalves/python-hcl2
 Author: João Gonçalves
 Author-email: joao.marques.goncalves@tecnico.ulisboa.pt
 License: MIT
+Platform: UNKNOWN
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
@@ -17,14 +18,16 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+[![Codacy Badge](https://app.codacy.com/project/badge/Grade/2e2015f9297346cbaa788c46ab957827)](https://app.codacy.com/gh/amplify-education/python-hcl2/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_grade)
+[![Build Status](https://travis-ci.org/amplify-education/python-hcl2.svg?branch=master)](https://travis-ci.org/amplify-education/python-hcl2)
 [![License](https://img.shields.io/badge/license-MIT-blue.svg)](https://raw.githubusercontent.com/amplify-education/python-hcl2/master/LICENSE)
 
 # Notice
 
 This is a fork of Amplify's [Python HCL2](https://github.com/amplify-education/python-hcl2) repository. This repository went through minor changes to work better with [GLITCH](https://github.com/sr-lab/GLITCH) and as the changes concern only the structure representation to be compatible with [GLITCH](https://github.com/sr-lab/GLITCH) we decided not to request updates for the upstream project. The two projects diverge in the representation of some structures and pushing new changes upstream doesn't make sense.
 
 # Python HCL2
@@ -94,7 +97,9 @@
 
 We welcome pull requests! For your pull request to be accepted smoothly, we suggest that you:
 
 - For any sizable change, first open a GitHub issue to discuss your idea.
 - Create a pull request.  Explain why you want to make the change and what it’s for.
 
 We’ll try to answer any PR’s promptly.
+
+
```

### Comparing `glitch-python-hcl2-0.1.4/hcl2/__main__.py` & `glitch-python-hcl2-0.2.0/hcl2/__main__.py`

 * *Files identical despite different names*

### Comparing `glitch-python-hcl2-0.1.4/hcl2/api.py` & `glitch-python-hcl2-0.2.0/hcl2/api.py`

 * *Files identical despite different names*

### Comparing `glitch-python-hcl2-0.1.4/hcl2/hcl2.lark` & `glitch-python-hcl2-0.2.0/hcl2/hcl2.lark`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 start : body
 body : (new_line_or_comment? (attribute | block))* new_line_or_comment?
 attribute : identifier "=" expression
-block : identifier (identifier | STRING_LIT)* "{" body "}"
+block : identifier (identifier | STRING_LIT)* new_line_or_comment? "{" body "}"
 new_line_and_or_comma: new_line_or_comment | "," | "," new_line_or_comment
 new_line_or_comment: ( /\n/ | /#.*\n/ | /\/\/.*\n/ | /\/\*(.|\n)*?(\*\/)/ )+
 
 identifier : /[a-zA-Z_][a-zA-Z0-9_-]*/
 
 ?expression : expr_term | operation | conditional
 
 conditional : expression "?" new_line_or_comment? expression new_line_or_comment? ":" new_line_or_comment? expression
 
 ?operation : unary_op | binary_op
 !unary_op : ("-" | "!") expr_term
-binary_op : expression binary_term
+binary_op : expression binary_term new_line_or_comment?
 !binary_operator : "==" | "!=" | "<" | ">" | "<=" | ">=" | "-" | "*" | "/" | "%" | "&&" | "||" | "+"
 binary_term : binary_operator new_line_or_comment? expression
 
 expr_term : "(" new_line_or_comment? expression new_line_or_comment? ")"
             | float_lit
             | int_lit
             | STRING_LIT
```

### Comparing `glitch-python-hcl2-0.1.4/hcl2/transformer.py` & `glitch-python-hcl2-0.2.0/hcl2/transformer.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,18 +10,23 @@
 
 HEREDOC_PATTERN = re.compile(r"<<([a-zA-Z][a-zA-Z0-9._-]+)\n([\s\S]*)\1", re.S)
 HEREDOC_TRIM_PATTERN = re.compile(r"<<-([a-zA-Z][a-zA-Z0-9._-]+)\n([\s\S]*)\1", re.S)
 
 
 START_LINE = "__start_line__"
 END_LINE = "__end_line__"
+START_COLUMN = "__start_column__"
+END_COLUMN = "__end_column__"
 COMMENTS = "__comments__"
 
 
-Attribute = namedtuple("Attribute", ("key", "value", "start_line", "end_line"))
+Attribute = namedtuple(
+    "Attribute",
+    ("key", "value", "start_line", "end_line", "start_column", "end_column"),
+)
 Comment = namedtuple("Comment", ("value", "start_line", "end_line"))
 
 comments = []
 id = None
 
 
 # pylint: disable=missing-function-docstring,unused-argument
@@ -104,15 +109,17 @@
         key = self.strip_quotes(args[0])
         value = self.to_string_dollar(args[1])
         d: Dict[str, Any] = {}
         d["value"] = value
         if self.with_meta:
             d[START_LINE] = meta.line
             d[END_LINE] = meta.end_line
-        return {key:d}
+            d[START_COLUMN] = meta.column
+            d[END_COLUMN] = meta.end_column
+        return {key: d}
 
     def object(self, args: List) -> Dict:
         args = self.strip_new_line_tokens(args)
         result: Dict[str, Any] = {}
 
         for arg in args:
             result.update(arg)
@@ -122,15 +129,15 @@
         def remove_meta_info(arg):
             if isinstance(arg, dict):
                 d = {}
                 for n, v in arg.items():
                     if isinstance(v, dict) or isinstance(v, list):
                         d[n] = remove_meta_info(v)
                     else:
-                        if n == START_LINE or n == END_LINE:
+                        if n in [START_LINE, END_LINE, START_COLUMN, END_COLUMN]:
                             continue
                         else:
                             d[n] = v
                 return d
             elif isinstance(arg, list):
                 l = []
                 for a in arg:
@@ -180,14 +187,16 @@
         *block_labels, block_body = args
         result: Dict[str, Any] = block_body
         if self.with_meta:
             result.update(
                 {
                     START_LINE: meta.line,
                     END_LINE: meta.end_line,
+                    START_COLUMN: meta.column,
+                    END_COLUMN: meta.end_column,
                 }
             )
 
         # create nested dict. i.e. {label1: {label2: {labelN: result}}}
         for label in reversed(block_labels):
             label_str = self.strip_quotes(label)
             result = {label_str: result}
@@ -197,16 +206,18 @@
     @v_args(meta=True)
     def attribute(self, meta: Meta, args: List) -> Attribute:
         key = str(args[0])
         if key.startswith('"') and key.endswith('"'):
             key = key[1:-1]
         value = self.to_string_dollar(args[1])
         if self.with_meta:
-            return Attribute(key, value, meta.line, meta.end_line)
-        return Attribute(key, value, 0, 0)
+            return Attribute(
+                key, value, meta.line, meta.end_line, meta.column, meta.end_column
+            )
+        return Attribute(key, value, 0, 0, 0, 0)
 
     def conditional(self, args: List) -> str:
         args = self.strip_new_line_tokens(args)
         return f"{args[0]} ? {args[1]} : {args[2]}"
 
     def binary_op(self, args: List) -> str:
         return " ".join([str(arg) for arg in args])
@@ -243,15 +254,15 @@
                 d: Dict[str, Any] = {}
                 d["value"] = c.value
                 if self.with_meta:
                     d[START_LINE] = c.start_line
                     d[END_LINE] = c.end_line
                 result[COMMENTS].append(d)
             comments = []
-        
+
         args = self.strip_new_line_tokens(args)
         attributes = set()
         result: Dict[str, Any] = {}
         global comments
         global id
 
         if args == [] and id == None and comments != []:
@@ -263,28 +274,41 @@
                 if arg.key in result:
                     raise RuntimeError(f"{arg.key} already defined")
                 d: Dict[str, Any] = {}
                 d["value"] = arg.value
                 if self.with_meta:
                     d[START_LINE] = arg.start_line
                     d[END_LINE] = arg.end_line
+                    d[START_COLUMN] = arg.start_column
+                    d[END_COLUMN] = arg.end_column
                 result[arg.key] = d
                 attributes.add(arg.key)
             else:
                 # This is a block.
                 for key, value in arg.items():
                     key = str(key)
                     if key in result:
                         if key in attributes:
                             raise RuntimeError(f"{key} already defined")
                         result[key].append(value)
                     else:
                         result[key] = [value]
-                    
-                    if key in ["resource", "data", "variable", "module", "output", "locals"] and comments != []:
+
+                    if (
+                        key
+                        in [
+                            "resource",
+                            "data",
+                            "variable",
+                            "module",
+                            "output",
+                            "locals",
+                        ]
+                        and comments != []
+                    ):
                         add_comments()
 
         return result
 
     def start(self, args: List) -> Dict:
         args = self.strip_new_line_tokens(args)
         return args[0]
@@ -325,30 +349,31 @@
         return '"%s"' % "\n".join(lines)
 
     @v_args(meta=True)
     def new_line_or_comment(self, meta: Meta, args: List) -> _DiscardType:
         global comments
         line = 0
         for arg in args:
-            if arg == '\n':
+            if arg == "\n":
                 line += 1
             else:
                 if self.with_meta:
                     start_line = meta.line + line
                     end_line = start_line + len(arg.splitlines()) - 1
                     comments.append(Comment(arg.value, start_line, end_line))
                 else:
                     comments.append(Comment(arg.value, 0, 0))
-                if len(arg.splitlines()) > 1:   
-                    line += len(arg.splitlines()) - 1 # multiline comment does not contain the final \n
-                else: 
+                if len(arg.splitlines()) > 1:
+                    line += (
+                        len(arg.splitlines()) - 1
+                    )  # multiline comment does not contain the final \n
+                else:
                     line += 1
-                
+
         return Discard
-            
 
     def for_tuple_expr(self, args: List) -> str:
         args = self.strip_new_line_tokens(args)
         for_expr = " ".join([str(arg) for arg in args[1:-1]])
         return f"[{for_expr}]"
 
     def for_intro(self, args: List) -> str:
```

### Comparing `glitch-python-hcl2-0.1.4/setup.py` & `glitch-python-hcl2-0.2.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,43 +1,50 @@
 import os.path
 from setuptools import setup, find_packages
 
+
 def get_long_description():
     """Reads the long description from the README"""
     this_directory = os.path.abspath(os.path.dirname(__file__))
-    with open(os.path.join(this_directory, 'README.md'), encoding='utf-8') as file:
+    with open(os.path.join(this_directory, "README.md"), encoding="utf-8") as file:
         return file.read()
 
+
 def get_requirements():
     """Reads the installation requirements from requirements.txt"""
-    with open("requirements.txt", encoding='utf8') as reqfile:
-        return [line for line in reqfile.read().split("\n") if not line.startswith(('#', '-'))]
+    with open("requirements.txt", encoding="utf8") as reqfile:
+        return [
+            line
+            for line in reqfile.read().split("\n")
+            if not line.startswith(("#", "-"))
+        ]
+
 
 setup(
-    name='glitch-python-hcl2',
-    version='0.1.4',
-    author='João Gonçalves',
-    author_email='joao.marques.goncalves@tecnico.ulisboa.pt',
+    name="glitch-python-hcl2",
+    version="0.2.0",
+    author="João Gonçalves",
+    author_email="joao.marques.goncalves@tecnico.ulisboa.pt",
     url="https://github.com/joaotgoncalves/python-hcl2",
-    license='MIT',
+    license="MIT",
     classifiers=[
-        'Topic :: Software Development :: Libraries :: Python Modules',
-        'Intended Audience :: Developers',
-        'License :: OSI Approved :: MIT License',
-        'Operating System :: OS Independent',
-        'Programming Language :: Python',
-        'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: 3.8',
-        'Programming Language :: Python :: 3.9',
-        'Programming Language :: Python :: 3.10',
-        'Programming Language :: Python :: 3.11',
+        "Topic :: Software Development :: Libraries :: Python Modules",
+        "Intended Audience :: Developers",
+        "License :: OSI Approved :: MIT License",
+        "Operating System :: OS Independent",
+        "Programming Language :: Python",
+        "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
     ],
-    keywords='',
-    python_requires='>=3.7', 
+    keywords="",
+    python_requires=">=3.7",
     packages=find_packages(),
     include_package_data=True,
     description="A parser for HCL2",
     long_description=get_long_description(),
-    long_description_content_type='text/markdown',
+    long_description_content_type="text/markdown",
     install_requires=get_requirements(),
-)
+)
```

