# Comparing `tmp/pyro-lexer-0.3.4.tar.gz` & `tmp/pyro-lexer-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyro-lexer-0.3.4.tar", last modified: Thu Oct 12 19:38:36 2023, max compression
+gzip compressed data, was "pyro-lexer-0.4.0.tar", last modified: Fri May 10 13:26:51 2024, max compression
```

## Comparing `pyro-lexer-0.3.4.tar` & `pyro-lexer-0.4.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 dmulholl   (501) staff       (20)        0 2023-10-12 19:38:36.269157 pyro-lexer-0.3.4/
--rw-r--r--   0 dmulholl   (501) staff       (20)      401 2023-10-12 19:38:36.268781 pyro-lexer-0.3.4/PKG-INFO
-drwxr-xr-x   0 dmulholl   (501) staff       (20)        0 2023-10-12 19:38:36.268260 pyro-lexer-0.3.4/pyro_lexer.egg-info/
--rw-r--r--   0 dmulholl   (501) staff       (20)      401 2023-10-12 19:38:36.000000 pyro-lexer-0.3.4/pyro_lexer.egg-info/PKG-INFO
--rw-r--r--   0 dmulholl   (501) staff       (20)      228 2023-10-12 19:38:36.000000 pyro-lexer-0.3.4/pyro_lexer.egg-info/SOURCES.txt
--rw-r--r--   0 dmulholl   (501) staff       (20)        1 2023-10-12 19:38:36.000000 pyro-lexer-0.3.4/pyro_lexer.egg-info/dependency_links.txt
--rw-r--r--   0 dmulholl   (501) staff       (20)       46 2023-10-12 19:38:36.000000 pyro-lexer-0.3.4/pyro_lexer.egg-info/entry_points.txt
--rw-r--r--   0 dmulholl   (501) staff       (20)       16 2023-10-12 19:38:36.000000 pyro-lexer-0.3.4/pyro_lexer.egg-info/requires.txt
--rw-r--r--   0 dmulholl   (501) staff       (20)       11 2023-10-12 19:38:36.000000 pyro-lexer-0.3.4/pyro_lexer.egg-info/top_level.txt
--rw-r--r--   0 dmulholl   (501) staff       (20)     2044 2023-10-12 19:28:12.000000 pyro-lexer-0.3.4/pyro_lexer.py
--rw-r--r--   0 dmulholl   (501) staff       (20)       38 2023-10-12 19:38:36.269328 pyro-lexer-0.3.4/setup.cfg
--rwxr-xr-x   0 dmulholl   (501) staff       (20)     1005 2023-04-01 18:43:25.000000 pyro-lexer-0.3.4/setup.py
+drwxr-xr-x   0 dmulholl   (501) staff       (20)        0 2024-05-10 13:26:51.917424 pyro-lexer-0.4.0/
+-rw-r--r--   0 dmulholl   (501) staff       (20)      432 2024-05-10 13:26:51.916849 pyro-lexer-0.4.0/PKG-INFO
+drwxr-xr-x   0 dmulholl   (501) staff       (20)        0 2024-05-10 13:26:51.916061 pyro-lexer-0.4.0/pyro_lexer.egg-info/
+-rw-r--r--   0 dmulholl   (501) staff       (20)      432 2024-05-10 13:26:51.000000 pyro-lexer-0.4.0/pyro_lexer.egg-info/PKG-INFO
+-rw-r--r--   0 dmulholl   (501) staff       (20)      228 2024-05-10 13:26:51.000000 pyro-lexer-0.4.0/pyro_lexer.egg-info/SOURCES.txt
+-rw-r--r--   0 dmulholl   (501) staff       (20)        1 2024-05-10 13:26:51.000000 pyro-lexer-0.4.0/pyro_lexer.egg-info/dependency_links.txt
+-rw-r--r--   0 dmulholl   (501) staff       (20)       46 2024-05-10 13:26:51.000000 pyro-lexer-0.4.0/pyro_lexer.egg-info/entry_points.txt
+-rw-r--r--   0 dmulholl   (501) staff       (20)       16 2024-05-10 13:26:51.000000 pyro-lexer-0.4.0/pyro_lexer.egg-info/requires.txt
+-rw-r--r--   0 dmulholl   (501) staff       (20)       11 2024-05-10 13:26:51.000000 pyro-lexer-0.4.0/pyro_lexer.egg-info/top_level.txt
+-rw-r--r--   0 dmulholl   (501) staff       (20)     2033 2024-03-17 17:11:33.000000 pyro-lexer-0.4.0/pyro_lexer.py
+-rw-r--r--   0 dmulholl   (501) staff       (20)       38 2024-05-10 13:26:51.917606 pyro-lexer-0.4.0/setup.cfg
+-rwxr-xr-x   0 dmulholl   (501) staff       (20)     1005 2023-04-01 18:43:25.000000 pyro-lexer-0.4.0/setup.py
```

### Comparing `pyro-lexer-0.3.4/pyro_lexer.py` & `pyro-lexer-0.4.0/pyro_lexer.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import re
 
 from pygments.lexer import RegexLexer, words
 from pygments.token import Text, Comment, Operator, Keyword, Name, String, Number, Punctuation
 
 __all__ = ['PyroLexer']
-__version__ = "0.3.4"
+__version__ = "0.4.0"
 
 class PyroLexer(RegexLexer):
     name = 'Pyro'
     filenames = ['*.pyro']
     aliases = ['pyro']
 
     flags = re.MULTILINE | re.UNICODE
@@ -17,21 +17,20 @@
         'root': [
             (r'\n', Text),
             (r'\s+', Text),
             (r'#(.*?)\n', Comment.Single),
             (r'(>>>|[.]{3})', Comment.Preproc),
 
             (r'(import|as)\b', Keyword.Namespace),
-            (r'(var|let|def|class|typedef|pub|pri|static|with)\b', Keyword.Declaration),
+            (r'(var|let|def|class|typedef|pub|pri|static|with|extends|enum|interface)\b', Keyword.Declaration),
 
             (words((
-                'if', 'else', 'for', 'in', 'loop', 'while',
+                'if', 'else', 'for', 'in', 'loop', 'while', 'defer',
                 'break', 'continue', 'return',
                 'echo', 'try', 'assert',
-                'and', 'or', 'xor', 'not',
             ), suffix=r'\b'), Keyword),
 
             (r'(true|false|null|self|super)\b', Keyword.Constant),
 
             # Float literal.
             (r'\d[\d_]*(\.[\d_]+[eE][+\-]?[\d_]+|\.[\d_]*|[eE][+\-]?[\d_]+)', Number.Float),
```

### Comparing `pyro-lexer-0.3.4/setup.py` & `pyro-lexer-0.4.0/setup.py`

 * *Files identical despite different names*

