# Comparing `tmp/combustache-1.2.0.tar.gz` & `tmp/combustache-2.0.0.tar.gz`

## Comparing `combustache-1.2.0.tar` & `combustache-2.0.0.tar`

### file list

```diff
@@ -1,29 +1,30 @@
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 combustache-1.2.0/.gitmodules
--rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 combustache-1.2.0/.github/workflows/ci.yaml
--rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 combustache-1.2.0/.github/workflows/publish.yaml
--rw-r--r--   0        0        0     1225 2020-02-02 00:00:00.000000 combustache-1.2.0/src/combustache/__init__.py
--rw-r--r--   0        0        0     2621 2020-02-02 00:00:00.000000 combustache-1.2.0/src/combustache/__main__.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 combustache-1.2.0/src/combustache/__version__.py
--rw-r--r--   0        0        0     1582 2020-02-02 00:00:00.000000 combustache-1.2.0/src/combustache/ctx.py
--rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 combustache-1.2.0/src/combustache/exceptions.py
--rw-r--r--   0        0        0     7474 2020-02-02 00:00:00.000000 combustache-1.2.0/src/combustache/main.py
--rw-r--r--   0        0        0     2635 2020-02-02 00:00:00.000000 combustache-1.2.0/src/combustache/util.py
--rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 combustache-1.2.0/src/combustache/nodes/__init__.py
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 combustache-1.2.0/src/combustache/nodes/comment.py
--rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 combustache-1.2.0/src/combustache/nodes/delimiter.py
--rw-r--r--   0        0        0     1485 2020-02-02 00:00:00.000000 combustache-1.2.0/src/combustache/nodes/interpolation.py
--rw-r--r--   0        0        0     2242 2020-02-02 00:00:00.000000 combustache-1.2.0/src/combustache/nodes/node.py
--rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 combustache-1.2.0/src/combustache/nodes/partial.py
--rw-r--r--   0        0        0     4618 2020-02-02 00:00:00.000000 combustache-1.2.0/src/combustache/nodes/section.py
--rw-r--r--   0        0        0     2263 2020-02-02 00:00:00.000000 combustache-1.2.0/tests/conftest.py
--rw-r--r--   0        0        0     1469 2020-02-02 00:00:00.000000 combustache-1.2.0/tests/custom/conftest.py
--rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 combustache-1.2.0/tests/custom/indexing.yml
--rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 combustache-1.2.0/tests/custom/test_bad_template.py
--rw-r--r--   0        0        0     3341 2020-02-02 00:00:00.000000 combustache-1.2.0/tests/custom/test_cli.py
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 combustache-1.2.0/tests/custom/test_misc.py
--rw-r--r--   0        0        0     2426 2020-02-02 00:00:00.000000 combustache-1.2.0/tests/custom/test_opts.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 combustache-1.2.0/.gitignore
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 combustache-1.2.0/LICENSE
--rw-r--r--   0        0        0     4721 2020-02-02 00:00:00.000000 combustache-1.2.0/README.md
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 combustache-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     6322 2020-02-02 00:00:00.000000 combustache-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 combustache-2.0.0/.gitmodules
+-rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 combustache-2.0.0/.github/workflows/ci.yaml
+-rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 combustache-2.0.0/.github/workflows/publish.yaml
+-rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 combustache-2.0.0/src/combustache/__init__.py
+-rw-r--r--   0        0        0     3051 2020-02-02 00:00:00.000000 combustache-2.0.0/src/combustache/__main__.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 combustache-2.0.0/src/combustache/__version__.py
+-rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 combustache-2.0.0/src/combustache/ctx.py
+-rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 combustache-2.0.0/src/combustache/exceptions.py
+-rw-r--r--   0        0        0     7528 2020-02-02 00:00:00.000000 combustache-2.0.0/src/combustache/main.py
+-rw-r--r--   0        0        0     3177 2020-02-02 00:00:00.000000 combustache-2.0.0/src/combustache/util.py
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 combustache-2.0.0/src/combustache/nodes/__init__.py
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 combustache-2.0.0/src/combustache/nodes/comment.py
+-rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 combustache-2.0.0/src/combustache/nodes/delimiter.py
+-rw-r--r--   0        0        0     4970 2020-02-02 00:00:00.000000 combustache-2.0.0/src/combustache/nodes/inheritance.py
+-rw-r--r--   0        0        0     1485 2020-02-02 00:00:00.000000 combustache-2.0.0/src/combustache/nodes/interpolation.py
+-rw-r--r--   0        0        0     2282 2020-02-02 00:00:00.000000 combustache-2.0.0/src/combustache/nodes/node.py
+-rw-r--r--   0        0        0      865 2020-02-02 00:00:00.000000 combustache-2.0.0/src/combustache/nodes/partial.py
+-rw-r--r--   0        0        0     4657 2020-02-02 00:00:00.000000 combustache-2.0.0/src/combustache/nodes/section.py
+-rw-r--r--   0        0        0     2180 2020-02-02 00:00:00.000000 combustache-2.0.0/tests/conftest.py
+-rw-r--r--   0        0        0     1469 2020-02-02 00:00:00.000000 combustache-2.0.0/tests/custom/conftest.py
+-rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 combustache-2.0.0/tests/custom/indexing.yml
+-rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 combustache-2.0.0/tests/custom/test_bad_template.py
+-rw-r--r--   0        0        0     3341 2020-02-02 00:00:00.000000 combustache-2.0.0/tests/custom/test_cli.py
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 combustache-2.0.0/tests/custom/test_misc.py
+-rw-r--r--   0        0        0     2426 2020-02-02 00:00:00.000000 combustache-2.0.0/tests/custom/test_opts.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 combustache-2.0.0/.gitignore
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 combustache-2.0.0/LICENSE
+-rw-r--r--   0        0        0     6147 2020-02-02 00:00:00.000000 combustache-2.0.0/README.md
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 combustache-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0     7748 2020-02-02 00:00:00.000000 combustache-2.0.0/PKG-INFO
```

### Comparing `combustache-1.2.0/.github/workflows/ci.yaml` & `combustache-2.0.0/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `combustache-1.2.0/.github/workflows/publish.yaml` & `combustache-2.0.0/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `combustache-1.2.0/src/combustache/__init__.py` & `combustache-2.0.0/src/combustache/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Cached Mustache v1.4 implementation with lambdas.
+Cached Mustache v1.4 implementation with all optional modules.
 
 Usable both in code and as CLI.
 To render a mustache template use `combustache.render`.
 To clear cache use `combustache.cache_clear`.
 To load templates/partials from a directory use `combustache.load_templates`.
 To work with template objects directly use `combustache.Template`.
 
@@ -26,20 +26,19 @@
 from combustache.exceptions import (
     CombustacheError,
     DelimiterError,
     MissingClosingTagError,
     StrayClosingTagError,
 )
 from combustache.main import Template, cache_clear, render
-from combustache.util import load_partials, load_templates
+from combustache.util import load_templates
 
 __all__ = [
     'render',
     'cache_clear',
     'Template',
     'CombustacheError',
     'DelimiterError',
     'MissingClosingTagError',
     'StrayClosingTagError',
-    'load_partials',
     'load_templates',
 ]
```

### Comparing `combustache-1.2.0/src/combustache/__main__.py` & `combustache-2.0.0/src/combustache/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,16 @@
 from combustache.main import render
 from combustache.util import find_template_files, paths_to_templates
 
 
 def cli(argv: Sequence[str] | None = None):
     parser = argparse.ArgumentParser(
         prog='combustache',
-        description='an explosive mustache v1.4 implementation with lambdas',
+        description='an explosive mustache v1.4 implementation with all'
+        ' optional modules',
     )
 
     parser.add_argument(
         '-v',
         '--version',
         action='version',
         version=__version__,
@@ -66,14 +67,21 @@
     parser.add_argument(
         '--partial-ext',
         default='.mustache',
         help="partial file extension (defaults to '.mustache')",
     )
 
     parser.add_argument(
+        '--include-relative-path',
+        action='store_true',
+        help="include template's relative path in its name"
+        ' (defaults to False)',
+    )
+
+    parser.add_argument(
         '--left-delimiter',
         default='{{',
         help="left mustache template delimiter (defaults to '{{')",
     )
 
     parser.add_argument(
         '--right-delimiter',
@@ -90,18 +98,27 @@
             template = f.read()
 
     data = json.load(args.data)
 
     if args.partial is None:
         args.partial = []
 
+    partials = paths_to_templates(
+        args.partial, args.partial_ext, False, Path('.')
+    )
+
     if args.partial_dir:
         partial_files = find_template_files(args.partial_dir, args.partial_ext)
-        args.partial.extend(partial_files)
-    partials = paths_to_templates(args.partial, args.partial_ext)
+        partials_from_dir = paths_to_templates(
+            partial_files,
+            args.partial_ext,
+            args.include_relative_path,
+            args.partial_dir,
+        )
+        partials.update(partials_from_dir)
 
     left_delimiter = args.left_delimiter
     right_delimiter = args.right_delimiter
 
     output = render(template, data, partials, left_delimiter, right_delimiter)
     args.output.write(output)
```

### Comparing `combustache-1.2.0/src/combustache/ctx.py` & `combustache-2.0.0/src/combustache/ctx.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,14 +4,18 @@
 
 
 class Ctx(list):
     """
     Context stack.
     """
 
+    def __init__(self, *args):
+        super().__init__(*args)
+        self.inheritance_args = {}
+
     def get(self, key: str) -> Any:
         """
         Gets a value from a context with a key.
 
         If nothing was found, combustache.ctx.MISSING is returned.
 
         Args:
```

### Comparing `combustache-1.2.0/src/combustache/main.py` & `combustache-2.0.0/src/combustache/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 import functools
 import html
 from typing import Any, Callable, Type
 
 from combustache.ctx import Ctx
 from combustache.nodes import (
     Ampersand,
+    Block,
     Closing,
     Comment,
     Delimiter,
     Interpolation,
     Inverted,
     Node,
+    Parent,
     Partial,
     Section,
     Triple,
 )
 from combustache.util import Opts, to_str
 
 _node_types: dict[str, type[Node]] = {
@@ -24,14 +26,16 @@
         Section,
         Ampersand,
         Inverted,
         Closing,
         Triple,
         Partial,
         Delimiter,
+        Block,
+        Parent,
     }
 }
 
 
 def find_node(
     template: str,
     search_start: int,
```

### Comparing `combustache-1.2.0/src/combustache/nodes/delimiter.py` & `combustache-2.0.0/src/combustache/nodes/delimiter.py`

 * *Files identical despite different names*

### Comparing `combustache-1.2.0/src/combustache/nodes/interpolation.py` & `combustache-2.0.0/src/combustache/nodes/interpolation.py`

 * *Files identical despite different names*

### Comparing `combustache-1.2.0/src/combustache/nodes/node.py` & `combustache-2.0.0/src/combustache/nodes/node.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,14 +35,15 @@
 
         # string between the last linebreak and node start
         self.before = template[line_start:tag_start]
         # string between node end and the next linebreak
         self.after = template[tag_end:line_end]
         # these are used to check if the tag is standalone
 
+        self.is_pair_standalone = False
         self.is_standalone = is_whitespace(self.before) and is_whitespace(
             self.after
         )
         if self.standalonable and self.is_standalone:
             self.start = line_start
             self.end = line_end
         else:
```

### Comparing `combustache-1.2.0/src/combustache/nodes/partial.py` & `combustache-2.0.0/src/combustache/nodes/partial.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,15 +6,19 @@
 
 class Partial(Node):
     left = '>'
 
     def handle(self, ctx: Ctx, partials: dict[str, str], opts: Opts) -> str:
         missing_data = opts['missing_data']
 
-        partial_template = partials.get(self.contents)
+        if self.contents[0] == '*':
+            partial_name = ctx.get(self.contents[1:].strip())
+            partial_template = partials.get(partial_name)
+        else:
+            partial_template = partials.get(self.contents)
 
         if partial_template is None:
             return missing_data()
 
         if self.is_standalone:
             partial_template = '\n'.join(
                 bool(line) * self.before + line
```

### Comparing `combustache-1.2.0/src/combustache/nodes/section.py` & `combustache-2.0.0/src/combustache/nodes/section.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,14 +63,15 @@
             end,
             self.template,
             self.template_start,
             self.template_end,
             self.left_delimiter,
             self.right_delimiter,
         )
+        self.closing_tag = closing_tag
 
         self.inside_start = self.end
         self.inside_end = closing_tag.start
         self.parse_end = closing_tag.end
         self.inside = combustache.main.Template(
             self.template,
             self.left_delimiter,
```

### Comparing `combustache-1.2.0/tests/conftest.py` & `combustache-2.0.0/tests/conftest.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,16 +14,15 @@
 
 
 yaml.add_constructor('!code', lambda_constructor)
 
 
 def pytest_collect_file(parent, file_path: Path):
     if file_path.suffix == '.yml':
-        if not file_path.name.startswith('~') or file_path.stem == '~lambdas':
-            return SpecFile.from_parent(parent, path=file_path)
+        return SpecFile.from_parent(parent, path=file_path)
 
 
 class SpecFile(pytest.File):
     def collect(self):
         with self.path.open() as f:
             r = yaml.load(f, yaml.Loader)
         for test in r['tests']:
```

### Comparing `combustache-1.2.0/tests/custom/conftest.py` & `combustache-2.0.0/tests/custom/conftest.py`

 * *Files identical despite different names*

### Comparing `combustache-1.2.0/tests/custom/indexing.yml` & `combustache-2.0.0/tests/custom/indexing.yml`

 * *Files identical despite different names*

### Comparing `combustache-1.2.0/tests/custom/test_bad_template.py` & `combustache-2.0.0/tests/custom/test_bad_template.py`

 * *Files identical despite different names*

### Comparing `combustache-1.2.0/tests/custom/test_cli.py` & `combustache-2.0.0/tests/custom/test_cli.py`

 * *Files identical despite different names*

### Comparing `combustache-1.2.0/tests/custom/test_opts.py` & `combustache-2.0.0/tests/custom/test_opts.py`

 * *Files identical despite different names*

### Comparing `combustache-1.2.0/.gitignore` & `combustache-2.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `combustache-1.2.0/LICENSE` & `combustache-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `combustache-1.2.0/README.md` & `combustache-2.0.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # combustache
 
 [![CI](https://github.com/sakhezech/combustache/actions/workflows/ci.yaml/badge.svg)](https://github.com/sakhezech/combustache/actions/workflows/ci.yaml)
 
-Cached Mustache v1.4 implementation with lambdas.
+Cached Mustache v1.4 implementation with all optional modules.
 
 Usable both in code and as CLI.
 To render a mustache template use `combustache.render`.
 To clear cache use `combustache.cache_clear`.
 To load templates/partials from a directory use `combustache.load_templates`.
 To work with template objects directly use `combustache.Template`.
 
@@ -20,51 +20,39 @@
 
 From git:
 
 ```sh
 pip install git+https://github.com/sakhezech/combustache
 ```
 
-## Usage as CLI
-
-`combustache ...` or `python -m combustache ...`
-
-```console
-$ combustache -h
-usage: combustache [-h] [-v] [-s] [-d DATA] [-o OUTPUT] [-p PARTIAL]
-                   [--partial-dir PARTIAL_DIR] [--partial-ext PARTIAL_EXT]
-                   [--left-delimiter LEFT_DELIMITER] [--right-delimiter RIGHT_DELIMITER]
-                   template
+## Usage in code
 
-an explosive mustache v1.4 implementation with lambdas
+### Loading templates/partials
 
-positional arguments:
-  template              mustache template file (use -s for string)
-
-options:
-  -h, --help            show this help message and exit
-  -v, --version         show program's version number and exit
-  -s, --string          pass in a string instead of a file for template
-  -d DATA, --data DATA  data json file (defaults to stdin)
-  -o OUTPUT, --output OUTPUT
-                        output file (defaults to stdout)
-  -p PARTIAL, --partial PARTIAL
-                        mustache partial file (can add multiple)
-  --partial-dir PARTIAL_DIR
-                        directory with mustache partials
-  --partial-ext PARTIAL_EXT
-                        partial file extension (defaults to '.mustache')
-  --left-delimiter LEFT_DELIMITER
-                        left mustache template delimiter (defaults to '{{')
-  --right-delimiter RIGHT_DELIMITER
-                        right mustache template delimiter (defaults to '}}')
+```py
+>>> # my_project/
+>>> # ├─ templates/
+>>> # │  ├─ ui/
+>>> # │  │  └─ comment.mustache
+>>> # │  ├─ index.mustache
+>>> # │  └─ other.file
+>>> # └─ ...
+>>> combustache.load_templates('./templates/', '.mustache')
+{
+    'comment': "<div class='comment'> {{content}} </div>",
+    'index': '<h1> Welcome, {{username}}! </h1>',
+}
+>>> combustache.load_templates('./templates/', '.mustache',
+... include_relative_path=True)
+{
+    'ui.comment': "<div class='comment'> {{content}} </div>",
+    'index': '<h1> Welcome, {{username}}! </h1>',
+}
 ```
 
-## Usage in code
-
 ### Basic
 
 ```py
 >>> template = 'Hello {{place}}!'
 >>> data = {'place': 'world'}
 >>> combustache.render(template, data)
 'Hello world!'
@@ -89,17 +77,46 @@
 ```py
 >>> template = 'My name is <%name%>.'
 >>> data = {'name': 'Anahit'}
 >>> combustache.render(template, data, left_delimiter='<%', right_delimiter='%>')
 'My name is Anahit.'
 ```
 
+### Lambda support
+
+```py
+>>> template = 'Hello, {{labmda}}!'
+>>> data = {'planet': 'world', 'labmda': lambda: '{{planet}}'}
+>>> combustache.render(template, data)
+'Hello, world!'
+```
+
+### Dynamic partials support
+
+```py
+>>> template = '{{>*dynamic}}'
+>>> data = {'dynamic': 'content'}
+>>> partials = {'content': 'something'}
+>>> combustache.render(template, data, partials)
+'something'
+```
+
+### Inheritance support
+
+```py
+>>> template = '{{< div}}{{$content}}hello :){{/content}}{{/ div}}'
+>>> data = {}
+>>> partials = {'div': '<div>{{$content}}default{{/content}}</div>'}
+>>> combustache.render(template, data, partials)
+'<div>hello :)</div>'
+```
+
 ### List indexing
 
-You can index into lists by dotting into them with a number. Both positive and negative numbers work.
+You can index into lists by dotting into them with a number.
 
 ```py
 >>> data = {'items': ['Apricot', 'Cherry', 'Pomegranate']}
 >>> template = 'The first item is {{items.0}}.'
 >>> combustache.render(template, data)
 'The first item is Apricot.'
 >>> template = 'The last item is {{items.-1}}.'
@@ -150,14 +167,53 @@
 ```py
 >>> template = '{{something}}'
 >>> data = {}
 >>> combustache.render(template, data, missing_data=lambda: 'NO DATA')
 'NO DATA'
 ```
 
+## Usage as CLI
+
+`combustache ...` or `python -m combustache ...`
+
+```console
+$ combustache -h
+usage: combustache [-h] [-v] [-s] [-d DATA] [-o OUTPUT] [-p PARTIAL]
+                   [--partial-dir PARTIAL_DIR] [--partial-ext PARTIAL_EXT]
+                   [--include-relative-path] [--left-delimiter LEFT_DELIMITER]
+                   [--right-delimiter RIGHT_DELIMITER]
+                   template
+
+an explosive mustache v1.4 implementation with all optional modules
+
+positional arguments:
+  template              mustache template file (use -s for string)
+
+options:
+  -h, --help            show this help message and exit
+  -v, --version         show program's version number and exit
+  -s, --string          pass in a string instead of a file for template
+  -d DATA, --data DATA  data json file (defaults to stdin)
+  -o OUTPUT, --output OUTPUT
+                        output file (defaults to stdout)
+  -p PARTIAL, --partial PARTIAL
+                        mustache partial file (can add multiple)
+  --partial-dir PARTIAL_DIR
+                        directory with mustache partials
+  --partial-ext PARTIAL_EXT
+                        partial file extension (defaults to '.mustache')
+  --include-relative-path
+                        include template's relative path in its name (defaults
+                        to False)
+  --left-delimiter LEFT_DELIMITER
+                        left mustache template delimiter (defaults to '{{')
+  --right-delimiter RIGHT_DELIMITER
+                        right mustache template delimiter (defaults to '}}')
+```
+
 ## Development
 
 Use `ruff check --fix .` and `ruff format .` to check and format your code.
 
 To get started:
 
 ```sh
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `combustache-1.2.0/pyproject.toml` & `combustache-2.0.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `combustache-1.2.0/PKG-INFO` & `combustache-2.0.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: combustache
-Version: 1.2.0
+Version: 2.0.0
 Summary: Mustache v1.4 implementation with lambdas.
 Project-URL: Homepage, https://github.com/sakhezech/combustache
 License: MIT License
         
         Copyright (c) 2023 Sakhezech
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -31,15 +31,15 @@
 Requires-Dist: ruff; extra == 'dev'
 Description-Content-Type: text/markdown
 
 # combustache
 
 [![CI](https://github.com/sakhezech/combustache/actions/workflows/ci.yaml/badge.svg)](https://github.com/sakhezech/combustache/actions/workflows/ci.yaml)
 
-Cached Mustache v1.4 implementation with lambdas.
+Cached Mustache v1.4 implementation with all optional modules.
 
 Usable both in code and as CLI.
 To render a mustache template use `combustache.render`.
 To clear cache use `combustache.cache_clear`.
 To load templates/partials from a directory use `combustache.load_templates`.
 To work with template objects directly use `combustache.Template`.
 
@@ -53,51 +53,39 @@
 
 From git:
 
 ```sh
 pip install git+https://github.com/sakhezech/combustache
 ```
 
-## Usage as CLI
-
-`combustache ...` or `python -m combustache ...`
-
-```console
-$ combustache -h
-usage: combustache [-h] [-v] [-s] [-d DATA] [-o OUTPUT] [-p PARTIAL]
-                   [--partial-dir PARTIAL_DIR] [--partial-ext PARTIAL_EXT]
-                   [--left-delimiter LEFT_DELIMITER] [--right-delimiter RIGHT_DELIMITER]
-                   template
+## Usage in code
 
-an explosive mustache v1.4 implementation with lambdas
+### Loading templates/partials
 
-positional arguments:
-  template              mustache template file (use -s for string)
-
-options:
-  -h, --help            show this help message and exit
-  -v, --version         show program's version number and exit
-  -s, --string          pass in a string instead of a file for template
-  -d DATA, --data DATA  data json file (defaults to stdin)
-  -o OUTPUT, --output OUTPUT
-                        output file (defaults to stdout)
-  -p PARTIAL, --partial PARTIAL
-                        mustache partial file (can add multiple)
-  --partial-dir PARTIAL_DIR
-                        directory with mustache partials
-  --partial-ext PARTIAL_EXT
-                        partial file extension (defaults to '.mustache')
-  --left-delimiter LEFT_DELIMITER
-                        left mustache template delimiter (defaults to '{{')
-  --right-delimiter RIGHT_DELIMITER
-                        right mustache template delimiter (defaults to '}}')
+```py
+>>> # my_project/
+>>> # ├─ templates/
+>>> # │  ├─ ui/
+>>> # │  │  └─ comment.mustache
+>>> # │  ├─ index.mustache
+>>> # │  └─ other.file
+>>> # └─ ...
+>>> combustache.load_templates('./templates/', '.mustache')
+{
+    'comment': "<div class='comment'> {{content}} </div>",
+    'index': '<h1> Welcome, {{username}}! </h1>',
+}
+>>> combustache.load_templates('./templates/', '.mustache',
+... include_relative_path=True)
+{
+    'ui.comment': "<div class='comment'> {{content}} </div>",
+    'index': '<h1> Welcome, {{username}}! </h1>',
+}
 ```
 
-## Usage in code
-
 ### Basic
 
 ```py
 >>> template = 'Hello {{place}}!'
 >>> data = {'place': 'world'}
 >>> combustache.render(template, data)
 'Hello world!'
@@ -122,17 +110,46 @@
 ```py
 >>> template = 'My name is <%name%>.'
 >>> data = {'name': 'Anahit'}
 >>> combustache.render(template, data, left_delimiter='<%', right_delimiter='%>')
 'My name is Anahit.'
 ```
 
+### Lambda support
+
+```py
+>>> template = 'Hello, {{labmda}}!'
+>>> data = {'planet': 'world', 'labmda': lambda: '{{planet}}'}
+>>> combustache.render(template, data)
+'Hello, world!'
+```
+
+### Dynamic partials support
+
+```py
+>>> template = '{{>*dynamic}}'
+>>> data = {'dynamic': 'content'}
+>>> partials = {'content': 'something'}
+>>> combustache.render(template, data, partials)
+'something'
+```
+
+### Inheritance support
+
+```py
+>>> template = '{{< div}}{{$content}}hello :){{/content}}{{/ div}}'
+>>> data = {}
+>>> partials = {'div': '<div>{{$content}}default{{/content}}</div>'}
+>>> combustache.render(template, data, partials)
+'<div>hello :)</div>'
+```
+
 ### List indexing
 
-You can index into lists by dotting into them with a number. Both positive and negative numbers work.
+You can index into lists by dotting into them with a number.
 
 ```py
 >>> data = {'items': ['Apricot', 'Cherry', 'Pomegranate']}
 >>> template = 'The first item is {{items.0}}.'
 >>> combustache.render(template, data)
 'The first item is Apricot.'
 >>> template = 'The last item is {{items.-1}}.'
@@ -183,14 +200,53 @@
 ```py
 >>> template = '{{something}}'
 >>> data = {}
 >>> combustache.render(template, data, missing_data=lambda: 'NO DATA')
 'NO DATA'
 ```
 
+## Usage as CLI
+
+`combustache ...` or `python -m combustache ...`
+
+```console
+$ combustache -h
+usage: combustache [-h] [-v] [-s] [-d DATA] [-o OUTPUT] [-p PARTIAL]
+                   [--partial-dir PARTIAL_DIR] [--partial-ext PARTIAL_EXT]
+                   [--include-relative-path] [--left-delimiter LEFT_DELIMITER]
+                   [--right-delimiter RIGHT_DELIMITER]
+                   template
+
+an explosive mustache v1.4 implementation with all optional modules
+
+positional arguments:
+  template              mustache template file (use -s for string)
+
+options:
+  -h, --help            show this help message and exit
+  -v, --version         show program's version number and exit
+  -s, --string          pass in a string instead of a file for template
+  -d DATA, --data DATA  data json file (defaults to stdin)
+  -o OUTPUT, --output OUTPUT
+                        output file (defaults to stdout)
+  -p PARTIAL, --partial PARTIAL
+                        mustache partial file (can add multiple)
+  --partial-dir PARTIAL_DIR
+                        directory with mustache partials
+  --partial-ext PARTIAL_EXT
+                        partial file extension (defaults to '.mustache')
+  --include-relative-path
+                        include template's relative path in its name (defaults
+                        to False)
+  --left-delimiter LEFT_DELIMITER
+                        left mustache template delimiter (defaults to '{{')
+  --right-delimiter RIGHT_DELIMITER
+                        right mustache template delimiter (defaults to '}}')
+```
+
 ## Development
 
 Use `ruff check --fix .` and `ruff format .` to check and format your code.
 
 To get started:
 
 ```sh
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

