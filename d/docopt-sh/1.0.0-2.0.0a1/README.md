# Comparing `tmp/docopt-sh-1.0.0.tar.gz` & `tmp/docopt_sh-2.0.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docopt-sh-1.0.0.tar", last modified: Sat Apr 23 12:39:57 2022, max compression
+gzip compressed data, was "docopt_sh-2.0.0a1.tar", max compression
```

## Comparing `docopt-sh-1.0.0.tar` & `docopt_sh-2.0.0a1.tar`

### file list

```diff
@@ -1,17 +1,10 @@
--rw-r--r--   0        0        0     1059 2022-04-23 12:39:38.442627 docopt-sh-1.0.0/LICENSE
--rw-r--r--   0        0        0    12288 2022-04-23 12:39:38.442627 docopt-sh-1.0.0/README.adoc
--rw-r--r--   0        0        0      551 2022-04-23 12:39:38.442627 docopt-sh-1.0.0/docopt_sh/__init__.py
--rw-r--r--   0        0        0     3574 2022-04-23 12:39:38.442627 docopt-sh-1.0.0/docopt_sh/__main__.py
--rw-r--r--   0        0        0     3238 2022-04-23 12:39:38.442627 docopt-sh-1.0.0/docopt_sh/bash.py
--rw-r--r--   0        0        0    11568 2022-04-23 12:39:38.442627 docopt-sh-1.0.0/docopt_sh/doc_ast.py
--rw-r--r--   0        0        0     9794 2022-04-23 12:39:38.442627 docopt-sh-1.0.0/docopt_sh/docopt.sh
--rw-r--r--   0        0        0     3009 2022-04-23 12:39:38.442627 docopt-sh-1.0.0/docopt_sh/node.py
--rw-r--r--   0        0        0     7488 2022-04-23 12:39:38.442627 docopt-sh-1.0.0/docopt_sh/parser.py
--rw-r--r--   0        0        0     8867 2022-04-23 12:39:38.442627 docopt-sh-1.0.0/docopt_sh/script.py
--rw-r--r--   0        0        0       22 2022-04-23 12:39:38.666640 docopt-sh-1.0.0/docopt_sh/version.py
--rw-r--r--   0        0        0      221 2022-04-23 12:39:38.442627 docopt-sh-1.0.0/docs/README.pypi.md
--rw-r--r--   0        0        0     2062 2022-04-23 12:39:38.442627 docopt-sh-1.0.0/docs/naval_fate.library.sh
--rw-r--r--   0        0        0     7665 2022-04-23 12:39:38.442627 docopt-sh-1.0.0/docs/naval_fate.patched.sh
--rw-r--r--   0        0        0      451 2022-04-23 12:39:38.442627 docopt-sh-1.0.0/docs/naval_fate.sh
--rw-r--r--   0        0        0      815 2022-04-23 12:39:38.442627 docopt-sh-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      928 1970-01-01 00:00:00.000000 docopt-sh-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1059 2024-05-10 10:12:23.956291 docopt_sh-2.0.0a1/LICENSE
+-rw-r--r--   0        0        0      602 2024-05-10 10:12:23.956291 docopt_sh-2.0.0a1/docopt_sh/__init__.py
+-rw-r--r--   0        0        0     3590 2024-05-10 10:12:23.956291 docopt_sh-2.0.0a1/docopt_sh/__main__.py
+-rw-r--r--   0        0        0     4011 2024-05-10 10:12:23.956291 docopt_sh-2.0.0a1/docopt_sh/bash.py
+-rw-r--r--   0        0        0    17437 2024-05-10 10:12:23.956291 docopt_sh-2.0.0a1/docopt_sh/docopt.sh
+-rw-r--r--   0        0        0    10211 2024-05-10 10:12:23.956291 docopt_sh-2.0.0a1/docopt_sh/parser.py
+-rw-r--r--   0        0        0     9063 2024-05-10 10:12:23.956291 docopt_sh-2.0.0a1/docopt_sh/script.py
+-rw-r--r--   0        0        0      221 2024-05-10 10:12:23.956291 docopt_sh-2.0.0a1/docs/README.pypi.md
+-rw-r--r--   0        0        0     1218 2024-05-10 10:12:35.792447 docopt_sh-2.0.0a1/pyproject.toml
+-rw-r--r--   0        0        0     1100 1970-01-01 00:00:00.000000 docopt_sh-2.0.0a1/PKG-INFO
```

### Comparing `docopt-sh-1.0.0/LICENSE` & `docopt_sh-2.0.0a1/LICENSE`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (c) 2019 Anders Ingemann
+Copyright (c) 2024 Anders Ingemann
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `docopt-sh-1.0.0/docopt_sh/__main__.py` & `docopt_sh-2.0.0a1/docopt_sh/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,13 +97,13 @@
     stderr.setFormatter(ColorFormatter())
   log.setLevel(level=logging.INFO)
   log.addHandler(stderr)
 
 
 def main():
   setup_logging()
-  params = docopt.docopt(__doc__, version=__version__)
+  params = docopt.docopt(__doc__, version=__version__)  # type: ignore
   docopt_sh(params)
 
 
 if __name__ == '__main__':
   main()
```

### Comparing `docopt-sh-1.0.0/docopt_sh/bash.py` & `docopt_sh-2.0.0a1/docopt_sh/bash.py`

 * *Files 14% similar despite different names*

```diff
@@ -77,14 +77,16 @@
 
 
 def minify(parser_str, max_length):
   lines = parser_str.split('\n')
   lines = remove_leading_spaces(lines)
   lines = remove_empty_lines(lines)
   lines = remove_comments(lines)
+  lines = continuate_spaces(lines)
+  lines = split_sq_strings(lines)
   lines = remove_newlines(lines, max_length)
   return '\n'.join(lines) + '\n'
 
 
 def remove_leading_spaces(lines):
   for line in lines:
     yield re.sub(r'^\s*', '', line)
@@ -94,39 +96,61 @@
   for line in lines:
     if line != '':
       yield line
 
 
 def remove_comments(lines):
   for line in lines:
-    if re.match(r'^\s*#', line) is None:
+    if re.match(r'\s*#', line) is None:
       yield line
 
 
+def continuate_spaces(lines):
+  for line in lines:
+    # Split whenever there's a space, but make sure to keep single quoted
+    # strings on one line
+    yield from re.sub(r"('[^']* [^']*')|( )", r'\1\2\\\n', line).split('\n')
+
+
+def split_sq_strings(lines):
+  for line in lines:
+    # Split every character in a single quoted string
+    yield from re.sub(
+      r"'([^']+)'",
+      lambda sq: ''.join(map(lambda c: f"'{c}'\\\n", sq.group(1))),
+      line,
+    ).split('\n')
+
+
 def remove_newlines(lines, max_length):
-  def needs_separator(line):
-    return re.search(r'; (then|do)$|else$|\{$', line) is None
+  def get_seperator(line):
+    return ';' if re.search(r'(then|do|else|\{)$', line) is None else ' '
 
   def has_continuation(line):
     return re.search(r'\\\s*$', line) is not None
 
   def remove_continuation(line):
-    return re.sub(r'\s*\\\s*$', '', line)
+    return re.sub(r'\\(\s*)$', r'\1', line)
 
   def combine(line1, line2):
     if has_continuation(line1):
-      return remove_continuation(line1) + ' ' + line2
-    if needs_separator(line1):
-      return line1 + '; ' + line2
-    else:
-      return line1 + ' ' + line2
+      return remove_continuation(line1) + line2
+    return line1 + get_seperator(line1) + line2
 
   previous = next(lines)
   for line in lines:
     combined = combine(previous, line)
+    combined = merge_sq_strings(combined)
     if len(combined) > max_length:
       yield previous
       previous = line
     else:
       previous = combined
   if previous:
     yield previous
+
+
+def merge_sq_strings(line):
+  # We don't need to look for more than a single pair, because
+  # all strings were on their own line and remove_newlines()
+  # merges one line at a time
+  return re.sub(r"'([^']+)''([^']+)'", r"'\1\2'", line)
```

### Comparing `docopt-sh-1.0.0/docopt_sh/doc_ast.py` & `docopt_sh-2.0.0a1/docopt_sh/parser.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,376 +1,273 @@
+import os.path
 import re
+import hashlib
+import logging
+import shlex
 from collections import OrderedDict
-from itertools import chain
-
-
-class DocAst(object):
-
-  def __init__(self, doc):
-    from .node import BranchNode, LeafNode
-    doc = doc
-    root, self.usage_match = parse_doc(doc)
-    node_map = OrderedDict([])
-    param_sort_order = [Option, Argument, Command]
-    unique_params = list(OrderedDict.fromkeys(root.flat(*param_sort_order)))
-    sorted_params = sorted(unique_params, key=lambda p: param_sort_order.index(type(p)))
-    # Enumerate leaf nodes first so that their function index & index in the params array match
-    for idx, param in enumerate(sorted_params):
-      node_map[param] = LeafNode(param, idx)
-    idx = len(node_map)
-    for pattern in iter(root):
-      if isinstance(pattern, BranchPattern) and pattern not in node_map:
-        node_map[pattern] = BranchNode(pattern, idx, node_map)
-        idx += 1
-
-    self.root_node = node_map[root]
-    self.nodes = node_map.values()
-
-
-def parse_doc(doc):
-  usage_sections = parse_section('usage:', doc)
-  if len(usage_sections) == 0:
-    raise DocoptLanguageError('"usage:" (case-insensitive) not found.')
-  if len(usage_sections) > 1:
-    raise DocoptLanguageError('More than one "usage:" (case-insensitive).')
-  usage, usage_match = usage_sections[0]
-  # Trim newlines in usage_match
-  match_fix = re.search(r'\A\n*(.+?)\n*\Z', usage, re.MULTILINE | re.DOTALL)
-  usage_match = usage_match.start(0) + match_fix.start(0), usage_match.start(0) + match_fix.end(0)
-
-  options = parse_defaults(doc)
-  pattern = parse_pattern(formal_usage(usage), options)
-  pattern_options = set(pattern.flat(Option))
-  for options_shortcut in pattern.flat(OptionsShortcut):
-    doc_options = parse_defaults(doc)
-    options_shortcut.children = list(set(doc_options) - pattern_options)
-
-  return pattern.fix(), usage_match
-
-
-class DocoptLanguageError(Exception):
-
-  """Error in construction of usage-message by developer."""
-
-
-class Pattern(object):
-
-  def __eq__(self, other):
-    return repr(self) == repr(other)
-
-  def __hash__(self):
-    return hash(repr(self))
-
-  def fix(self):
-    self.fix_identities()
-    self.fix_repeating_arguments()
-    return self
-
-  def fix_identities(self, uniq=None):
-    """Make pattern-tree tips point to same object if they are equal."""
-    if not hasattr(self, 'children'):
-      return self
-    uniq = list(set(self.flat())) if uniq is None else uniq
-    for i, child in enumerate(self.children):
-      if not hasattr(child, 'children'):
-        assert child in uniq
-        self.children[i] = uniq[uniq.index(child)]
-      else:
-        child.fix_identities(uniq)
-
-  def fix_repeating_arguments(self):
-    """Fix elements that should accumulate/increment values."""
-    either = [list(child.children) for child in transform(self).children]
-    for case in either:
-      for e in [child for child in case if case.count(child) > 1]:
-        if type(e) is Argument or type(e) is Option and e.argcount:
-          if e.value is None:
-            e.value = []
-          elif type(e.value) is not list:
-            e.value = e.value.split()
-        if type(e) is Command or type(e) is Option and e.argcount == 0:
-          e.value = 0
-    return self
-
-
-def transform(pattern):
-  """Expand pattern into an (almost) equivalent one, but with single Either.
-
-  Example: ((-a | -b) (-c | -d)) => (-a -c | -a -d | -b -c | -b -d)
-  Quirks: [-a] => (-a), (-a...) => (-a -a)
-
-  """
-  result = []
-  groups = [[pattern]]
-  while groups:
-    children = groups.pop(0)
-    parents = [Required, Optional, OptionsShortcut, Either, OneOrMore]
-    if any(t in map(type, children) for t in parents):
-      child = [c for c in children if type(c) in parents][0]
-      children.remove(child)
-      if type(child) is Either:
-        for c in child.children:
-          groups.append([c] + children)
-      elif type(child) is OneOrMore:
-        groups.append(child.children * 2 + children)
-      else:
-        groups.append(child.children + children)
+from . import __version__, DocoptError
+import docopt_parser as P
+from .bash import Code, indent, bash_variable_name, bash_variable_value, bash_ifs_value
+from shlex import quote
+
+log = logging.getLogger(__name__)
+
+
+def get_leaves(memo, pattern):
+  if isinstance(pattern, P.Leaf):
+    memo.append(pattern)
+  return memo
+
+
+def get_groups(memo, pattern):
+  if isinstance(pattern, P.Group):
+    memo.append(pattern)
+  return memo
+
+
+class Parser(object):
+
+  def __init__(self, parser_parameters):
+    self.parameters = parser_parameters
+    self.library = Library()
+
+  def generate(self, script):
+    root = P.parse(script.doc.trimmed_value)
+    root = P.merge_identical_leaves(root, ignore_option_args=True)
+    root = P.merge_identical_groups(root)
+    root = P.collapse_groups(root)
+    (usage_start, usage_end) = root.mark.to_bytecount(script.doc.trimmed_value)
+
+    all_nodes = (
+      list(OrderedDict.fromkeys(root.reduce(get_leaves, [])))
+      + list(OrderedDict.fromkeys(root.reduce(get_groups, [])))
+    )
+    node_sort_order = [P.Option, P.Argument, P.Command, P.ArgumentSeparator]
+    nodes = sorted(
+      all_nodes,
+      key=lambda p: node_sort_order.index(type(p)) if type(p) in node_sort_order else len(node_sort_order)
+    )
+
+    if self.parameters.library_path:
+      library = indent(f'''source {self.parameters.library_path} '{__version__}' || {{
+  ret=$?
+  printf -- "exit %d\\n" "$ret"
+  exit "$ret"
+}}''', level=1)
     else:
-      result.append(children)
-  return Either(*[Required(*e) for e in result])
-
-
-class LeafPattern(Pattern):
-
-  """Leaf/terminal node of a pattern tree."""
-
-  def __init__(self, name, value=None):
-    self.name, self.value = name, value
-
-  def __repr__(self):
-    return '%s(%r, %r)' % (self.__class__.__name__, self.name, self.value)
-
-  def __iter__(self):
-    yield self
-
-  def flat(self, *types):
-    return [self] if not types or type(self) in types else []
-
-
-class BranchPattern(Pattern):
-
-  """Branch/inner node of a pattern tree."""
-
-  def __init__(self, *children):
-    self.children = list(children)
-
-  def __repr__(self):
-    return '%s(%s)' % (self.__class__.__name__, ', '.join(repr(a) for a in self.children))
-
-  def __iter__(self):
-    for child in chain(*map(iter, self.children)):
-      yield child
-    yield self
-
-  def flat(self, *types):
-    if type(self) in types:
-      return [self]
-    return sum([child.flat(*types) for child in self.children], [])
-
-
-class Argument(LeafPattern):
-
-  @classmethod
-  def parse(class_, source):
-    name = re.findall(r'(<\S*?>)', source)[0]
-    value = re.findall(r'\[default: (.*)\]', source, flags=re.I)
-    return class_(name, value[0] if value else None)
-
-
-class Command(Argument):
-
-  def __init__(self, name, value=False):
-    self.name, self.value = name, value
-
+      exclude = ['docopt', 'lib_version_check'] + list(set(helper_list) - set(map(helper_name, nodes)))
+      library = indent(str(self.library.generate_code(exclude=exclude)), level=1)
 
-class Option(LeafPattern):
-
-  def __init__(self, short=None, long=None, argcount=0, value=False):
-    assert argcount in (0, 1)
-    self.short, self.long, self.argcount = short, long, argcount
-    self.value = None if value is False and argcount else value
-
-  @classmethod
-  def parse(class_, option_description):
-    short, long, argcount, value = None, None, 0, False
-    options, _, description = option_description.strip().partition('  ')
-    options = options.replace(',', ' ').replace('=', ' ')
-    for s in options.split():
-      if s.startswith('--'):
-        long = s
-      elif s.startswith('-'):
-        short = s
-      else:
-        argcount = 1
-    if argcount:
-      matched = re.findall(r'\[default: (.*)\]', description, flags=re.I)
-      value = matched[0] if matched else None
-    return class_(short, long, argcount, value)
-
-  @property
-  def name(self):
-    return self.long or self.short
-
-  def __repr__(self):
-    return 'Option(%r, %r, %r, %r)' % (self.short, self.long, self.argcount, self.value)
-
-
-class Required(BranchPattern):
-  pass
-
-
-class Optional(BranchPattern):
-  pass
-
-
-class OptionsShortcut(Optional):
-  """Marker/placeholder for [options] shortcut."""
-
-
-class OneOrMore(BranchPattern):
-  pass
-
-
-class Either(BranchPattern):
-  pass
+    leaf_nodes = [node for node in nodes if isinstance(node, P.Leaf)]
 
+    replacements = {
+      '  "LIBRARY"': library,
+      '"DOC VALUE"': '${{DOC:{start}:{length}}}'.format(
+        start=script.doc.trimmed_value_start,
+        length=len(script.doc.trimmed_value),
+      ),
+      '"DOC USAGE"': '${{DOC:{start}:{length}}}'.format(
+        start=script.doc.trimmed_value_start + usage_start,
+        length=usage_end - usage_start,
+      ),
+      '"DOC DIGEST"': hashlib.sha256(script.doc.untrimmed_value.encode('utf-8')).hexdigest()[0:5],
+      '"OPTIONS"': generate_options_array(leaf_nodes),
+      '  "NODES"': indent('\n'.join(map(str, map(lambda n: ast_cmd(n, nodes), nodes))), level=1),
+      '"VARNAMES"': ' '.join([bash_ifs_value(var_name(node)) for node in leaf_nodes]),
+      '  "OUTPUT VARNAMES ASSIGNMENTS"': generate_default_assignments(leaf_nodes),
+      '  "EARLY RETURN"\n': '' if leaf_nodes else '  return 0\n',
+      '"ROOT NODE IDX"': len(nodes) - 1,
+    }
+    main = self.library.functions['docopt'].replace_literal(replacements)
+    if self.parameters.minify:
+      main = main.minify(self.parameters.max_line_length)
+
+    shellcheck_ignores = [
+      '2016',  # Ignore unexpanded variables in single quotes (used for docopt_exit generation)
+      '2086',  # Ignore unquoted vars, the DOCOPT_PREFIX var is unquoted to save some space
+      '2317',  # Ignore unreachable code, the parse functions are invoked via "node_$idx"
+    ]
+    if self.parameters.library_path:
+      shellcheck_ignores.extend([
+        '1090',  # Ignore non-constant library sourcing
+        '1091',  # Ignore library sourcing
+        '2034',  # Ignore unused vars (they refer to things in the library)
+      ])
+    if not self.parameters.library_path and self.parameters.minify:
+      # Ignore else .. if issue in parse_long,
+      # see https://github.com/koalaman/shellcheck/issues/1584 for more details
+      shellcheck_ignores.append('1075')
+    if any([type(node.default) is list for node in leaf_nodes]):  # type: ignore
+      # Unlike non-array values, array values will output a "declare -p var_..."
+      # to check in what way they should be set (${var:-VAL} does not work with arrays)
+      # So we ignore the "referenced but not assigned" error
+      shellcheck_ignores.append('2154')
+
+    return "{shellcheck_ignores}\n{parser}".format(
+      shellcheck_ignores='# shellcheck disable=%s' % ','.join(shellcheck_ignores),
+      parser=main,
+    )
+
+
+class Library(object):
+
+  def __init__(self):
+    function_re = re.compile((
+        r'^(?P<name>[a-z_][a-z0-9_]*)\(\)\s*\{'
+        r'\n+'
+        r'(?P<body>.*?)'
+        r'\n+\}\n$'
+      ), re.MULTILINE | re.IGNORECASE | re.DOTALL)
+    self.functions = OrderedDict([])
+    with open(os.path.join(os.path.dirname(__file__), 'docopt.sh'), 'r') as handle:
+      for match in function_re.finditer(handle.read()):
+        name = match.group('name')
+        if name == 'lib_version_check':
+          self.functions['lib_version_check'] = Code(match.group('body')).replace_literal(
+            {'"LIBRARY VERSION"': __version__}
+          )
+        else:
+          self.functions[match.group('name')] = Code(match.group(0))
 
-class Tokens(list):
+  def generate_code(self, exclude=[]):
+    return Code([code for name, code in self.functions.items() if name not in exclude])
 
-  def __init__(self, source):
-    self += source.split() if hasattr(source, 'split') else source
 
-  @staticmethod
-  def from_pattern(source):
-    source = re.sub(r'([\[\]\(\)\|]|\.\.\.)', r' \1 ', source)
-    source = [s for s in re.split(r'\s+|(\S*<.*?>)', source) if s]
-    return Tokens(source)
+class ParserParameter(object):
 
-  def move(self):
-    return self.pop(0) if len(self) else None
+  def __init__(self, name, invocation_params, script_params, default):
+    if script_params is None:
+      script_value = None
+    else:
+      script_value = script_params[name]
+    defined_in_invocation = invocation_params[name] is not None
+    defined_in_script = script_value is not None
+    auto_params = not invocation_params['--no-auto-params']
+
+    self.name = name
+    self.defined = (defined_in_invocation or defined_in_script) and auto_params
+    self.invocation_value = invocation_params[name] if defined_in_invocation else default
+    self.script_value = script_value if defined_in_script else default
+    self.merged_from_script = not defined_in_invocation and auto_params and defined_in_script
+    self.value = self.script_value if self.merged_from_script else self.invocation_value
+    self.changed = script_params is not None and self.value != self.script_value
+
+  def __str__(self):
+    return '%s=%s' % (self.name, shlex.quote(self.value))
+
+
+class ParserParameters(object):
+
+  def __init__(self, invocation_params, script=None):
+    if script is not None:
+      script_params = script.guards.bottom.refresh_command_params
+      if script_params is None:
+        if script.guards.present and not invocation_params['--no-auto-params']:
+          raise DocoptError(
+            'Unable to auto-detect parser generation parameters. '
+            'Re-run docopt.sh with `--no-auto-params`.'
+          )
+    else:
+      script_params = None
 
-  def current(self):
-    return self[0] if len(self) else None
+    params = OrderedDict([])
+    params['--line-length'] = ParserParameter('--line-length', invocation_params, script_params, default='80')
+    params['--library'] = ParserParameter('--library', invocation_params, script_params, default=None)
+
+    merged_from_script = list(filter(lambda p: p.merged_from_script, params.values()))
+    if merged_from_script:
+      log.info(
+        'Adding `%s` from parser generation parameters that were detected in the script. '
+        'Use --no-auto-params to disable this behavior.',
+        ' '.join(map(str, merged_from_script))
+      )
+
+    self.max_line_length = int(params['--line-length'].value)
+    self.library_path = params['--library'].value
+    self.minify = self.max_line_length > 0
+
+    command = ['docopt.sh']
+    command_short = ['docopt.sh']
+    if params['--line-length'].defined:
+      command.append(str(params['--line-length']))
+    if params['--library'].defined:
+      command.append(str(params['--library']))
+    if script is not None and script.path:
+      command.append(os.path.basename(script.path))
+      command_short.append(os.path.basename(script.path))
+    else:
+      command.append('-')
+      command.append('<FILE')
+      command_short.append('-')
+      command_short.append('<FILE')
+    self.refresh_command = ' '.join(command)
+    self.refresh_command_short = ' '.join(command_short)
+
+
+helper_list = ['sequence', 'choice', 'optional', 'repeatable', 'value', 'switch']
+
+
+def helper_name(node):
+  if isinstance(node, P.Group):
+    return {
+      P.Sequence: 'sequence',
+      P.Choice: 'choice',
+      P.Optional: 'optional',
+      P.Repeatable: 'repeatable',
+    }[type(node)]  # type: ignore
+  elif type(node) is P.Argument or type(node.default) not in [bool, int]:
+    return 'value'
+  else:
+    return 'switch'
 
 
-def parse_long(tokens, options):
-  """long ::= '--' chars [ ( ' ' | '=' ) chars ] ;"""
-  long, eq, value = tokens.move().partition('=')
-  assert long.startswith('--')
-  value = None if eq == value == '' else value
-  similar = [o for o in options if o.long == long]
-  if len(similar) > 1:  # might be simply specified ambiguously 2+ times?
-    raise DocoptLanguageError('%s is not a unique prefix: %s?' % (long, ', '.join(o.long for o in similar)))
-  elif len(similar) < 1:
-    argcount = 1 if eq == '=' else 0
-    o = Option(None, long, argcount)
-    options.append(o)
+def ast_cmd(node, sorted_nodes):
+  idx = sorted_nodes.index(node)
+  if isinstance(node, P.Group):
+    args = ' '.join([str(sorted_nodes.index(item)) for item in node.items])
   else:
-    o = Option(similar[0].short, similar[0].long, similar[0].argcount, similar[0].value)
-    if o.argcount == 0:
-      if value is not None:
-        raise DocoptLanguageError('%s must not have an argument' % o.long)
+    args = var_name(node)
+    if type(node) is P.Argument:
+      args += ' ' + bash_ifs_value('a')
     else:
-      if value is None:
-        if tokens.current() in [None, '--']:
-          raise DocoptLanguageError('%s requires argument' % o.long)
-        value = tokens.move()
-  return [o]
-
-
-def parse_shorts(tokens, options):
-  """shorts ::= '-' ( chars )* [ [ ' ' ] chars ] ;"""
-  token = tokens.move()
-  assert token.startswith('-') and not token.startswith('--')
-  left = token.lstrip('-')
-  parsed = []
-  while left != '':
-    short, left = '-' + left[0], left[1:]
-    similar = [o for o in options if o.short == short]
-    if len(similar) > 1:
-      raise DocoptLanguageError('%s is specified ambiguously %d times' % (short, len(similar)))
-    elif len(similar) < 1:
-      o = Option(short, None, 0)
-      options.append(o)
-    else:  # why copying is necessary here?
-      o = Option(short, similar[0].long, similar[0].argcount, similar[0].value)
-      if o.argcount != 0:
-        if left == '':
-          if tokens.current() in [None, '--']:
-            raise DocoptLanguageError('%s requires argument' % short)
-          tokens.move()
-        else:
-          left = ''
-    parsed.append(o)
-  return parsed
-
-
-def parse_pattern(source, options):
-  tokens = Tokens.from_pattern(source)
-  result = parse_expr(tokens, options)
-  if tokens.current() is not None:
-    raise DocoptLanguageError('unexpected ending: %r' % ' '.join(tokens))
-  return Required(*result)
-
-
-def parse_expr(tokens, options):
-  """expr ::= seq ( '|' seq )* ;"""
-  seq = parse_seq(tokens, options)
-  if tokens.current() != '|':
-    return seq
-  result = [Required(*seq)] if len(seq) > 1 else seq
-  while tokens.current() == '|':
-    tokens.move()
-    seq = parse_seq(tokens, options)
-    result += [Required(*seq)] if len(seq) > 1 else seq
-  return [Either(*result)] if len(result) > 1 else result
-
-
-def parse_seq(tokens, options):
-  """seq ::= ( atom [ '...' ] )* ;"""
-  result = []
-  while tokens.current() not in [None, ']', ')', '|']:
-    atom = parse_atom(tokens, options)
-    if tokens.current() == '...':
-      atom = [OneOrMore(*atom)]
-      tokens.move()
-    result += atom
-  return result
-
-
-def parse_atom(tokens, options):
-  """atom ::= '(' expr ')' | '[' expr ']' | 'options'
-       | long | shorts | argument | command ;
-  """
-  token = tokens.current()
-  result = []
-  if token in '([':
-    tokens.move()
-    matching, pattern = {'(': [')', Required], '[': [']', Optional]}[token]
-    result = pattern(*parse_expr(tokens, options))
-    if tokens.move() != matching:
-      raise DocoptLanguageError("unmatched '%s'" % token)
-    return [result]
-  elif token == 'options':
-    tokens.move()
-    return [OptionsShortcut()]
-  elif token.startswith('--') and token != '--':
-    return parse_long(tokens, options)
-  elif token.startswith('-') and token not in ('-', '--'):
-    return parse_shorts(tokens, options)
-  elif token.startswith('<') and token.endswith('>') or token.isupper():
-    return [Argument(tokens.move())]
-  else:
-    return [Command(tokens.move())]
-
+      args += ' ' + bash_ifs_value(idx if type(node) is P.Option else f'a:{node.ident}')
+    if type(node.default) in [list, int]:
+      args += ' true'
+  return Code(f'node_{idx}(){{\n  {helper_name(node)} {args}\n}}\n')
+
+
+def var_name(node):
+  return bash_variable_name(
+    node.definition.ident if isinstance(node, P.Option) else node.ident
+  )
+
+
+def generate_options_array(leaf_nodes):
+  return ' '.join([bash_ifs_value(' '.join([
+    node.short_alias or '',
+    node.definition.ident if node.definition.ident.startswith('--') else '',
+    '1' if node.argname else '0',
+  ])) for node in leaf_nodes if type(node) is P.Option])
+
+
+def generate_default_assignments(leaf_nodes):
+  list_assignments = []
+  value_assignments = []
+  for node in leaf_nodes:
+    variable_name = var_name(node)
+    if type(node.default) is list:
+      reassignment = f'{variable_name}=("${{var_{variable_name}[@]}}")'
+      default_assignment = f'{variable_name}={bash_variable_value(node.default)}'
+      list_assignments.append(
+        f'if declare -p var_{variable_name} >/dev/null 2>&1; then\n'
+        f'  eval $p{quote(reassignment)}\n'
+        'else\n'
+        f'  eval $p{quote(default_assignment)}\n'
+        'fi'
+      )
+    else:
+      assignment = f'{variable_name}=${{var_{variable_name}:-{bash_variable_value(node.default)}}};'
+      value_assignments.append(f'$p{quote(assignment)}')
+  joined_list_assignments = '\n'.join(list_assignments)
+  joined_value_assignments = 'eval ' + '\\\n'.join(value_assignments) + '\n'
 
-def parse_defaults(doc):
-  defaults = []
-  for s, _ in parse_section('options:', doc):
-    # FIXME corner case "bla: options: --foo"
-    _, _, s = s.partition(':')  # get rid of "options:"
-    split = re.split(r'\n[ \t]*(-\S+?)', '\n' + s)[1:]
-    split = [s1 + s2 for s1, s2 in zip(split[::2], split[1::2])]
-    options = [Option.parse(s) for s in split if s.startswith('-')]
-    defaults += options
-  return defaults
-
-
-def parse_section(name, source):
-  pattern = re.compile('^([^\n]*' + name + '[^\n]*\n?(?:[ \t].*?(?:\n|$))*)', re.IGNORECASE | re.MULTILINE)
-  return [(m.group(0).strip(), m) for m in pattern.finditer(source)]
-
-
-def formal_usage(section):
-  _, _, section = section.partition(':')  # drop "usage:"
-  pu = section.split()
-  return '( ' + ' '.join(') | (' if s == pu[0] else s for s in pu[1:]) + ' )'
+  return indent(joined_list_assignments + '\n' + joined_value_assignments, level=1)
```

### Comparing `docopt-sh-1.0.0/docopt_sh/script.py` & `docopt_sh-2.0.0a1/docopt_sh/script.py`

 * *Files 6% similar despite different names*

```diff
@@ -60,15 +60,15 @@
     if not self.invocation.present:
       log.warning(
         '%s No invocations of docopt found, check your script to make sure this is correct.\n'
         'docopt.sh is invoked with `eval "$(docopt "$@")"`.',
         self.invocation
       )
     for option in self.options:
-      if self.invocation.present and option.present and option.start > self.invocation.last.end:
+      if self.invocation.present and option.present and option.start > self.invocation.last.end:  # type: ignore
         log.warning(
           '%s $%s has no effect when specified after invoking docopt, '
           'make sure to place docopt options before calling `eval "$(docopt "$@")"`.',
           option, option.name
         )
 
   def patch(self, parser):
@@ -98,34 +98,34 @@
   def __init__(self, script, matches, offset):
     self.script = script
     self.matches = list(matches)
     self.match = self.matches[0] if self.matches else None
     self.offset = offset
     self.present = self.match is not None
     self.count = len(self.matches)
-    self.start = self.match.start(0) + (self.offset or 0) if self.present else None
-    self.end = self.match.end(0) + (self.offset or 0) if self.present else None
+    self.start = self.match.start(0) + (self.offset or 0) if self.present else None  # type: ignore
+    self.end = self.match.end(0) + (self.offset or 0) if self.present else None  # type: ignore
     self.line = self.script.contents[:self.start].count('\n') + 1
     self.all = [self] + [ScriptLocation(self.script, iter([match]), self.offset) for match in self.matches[1:]]
     if self.count == 0:
       self.last = None
     elif self.count == 1:
       self.last = self
     else:
       self.last = ScriptLocation(self.script, iter([self.matches[-1]]), self.offset)
 
   def __len__(self):
-    return self.end - self.start if self.present else 0
+    return self.end - self.start if self.present else 0  # type: ignore
 
   def __str__(self):
     path = self.script.path if self.script.path is not None else 'STDIN'
     if not self.present:
       return '%s' % (path)
     if self.count > 1:
-      return '%s:%s' % (path, ','.join(map(lambda l: str(l.line), self.all)))
+      return '%s:%s' % (path, ','.join(map(lambda loc: str(loc.line), self.all)))
     else:
       return '%s:%d' % (path, self.line)
 
 
 class Doc(ScriptLocation):
 
   def __init__(self, script):
@@ -143,32 +143,32 @@
       script.contents,
       re.MULTILINE | re.DOTALL
     )
     super(Doc, self).__init__(script, matches, 0)
     if self.present:
       # Get bash to output what the docstring looks like when evaluated
       output_doc = 'DOC={quote}{trimmed_raw_value}{quote};printf "%s" "$DOC"'.format(
-        trimmed_raw_value=self.match.group('trimmed_raw_value'),
-        quote=self.match.group('quote_start')
+        trimmed_raw_value=self.match.group('trimmed_raw_value'),  # type: ignore
+        quote=self.match.group('quote_start')  # type: ignore
       )
       process = subprocess.run(
         ['bash', '-c', 'eval "$(cat)"'],
         input=output_doc.encode('utf-8'),
         stdout=subprocess.PIPE, stderr=subprocess.PIPE
       )
       if process.returncode != 0:
         raise DocoptScriptValidationError(
           self, 'Unable to evaluate DOC= with system bash: %s' % process.stderr.decode('utf-8')
         )
       self.trimmed_value = process.stdout.decode('utf-8')
-      self.trimmed_value_start = self.match.start('trimmed_raw_value') - self.match.end('quote_start')
+      self.trimmed_value_start = self.match.start('trimmed_raw_value') - self.match.end('quote_start')  # type: ignore
       self.untrimmed_value = (
-        self.match.group('trimmed_before')
+        self.match.group('trimmed_before')  # type: ignore
         + self.trimmed_value
-        + self.match.group('trimmed_after')
+        + self.match.group('trimmed_after')  # type: ignore
       )
     else:
       self.value = None
 
 
 class TopGuard(ScriptLocation):
 
@@ -187,18 +187,18 @@
     matches = re.finditer(
       r'# docopt parser above(, complete command for generating this parser is `([^`]+)`)?.*\n',
       script.contents[offset:],
       re.MULTILINE
     )
     super(BottomGuard, self).__init__(script, matches, offset)
     self.refresh_command_params = None
-    if self.present and self.match.group(2) is not None:
+    if self.present and self.match.group(2) is not None:  # type: ignore
       from .__main__ import __doc__
       try:
-        self.refresh_command_params = docopt.docopt(__doc__, shlex.split(self.match.group(2))[1:])
+        self.refresh_command_params = docopt.docopt(__doc__, shlex.split(self.match.group(2))[1:])  # type: ignore
       except (docopt.DocoptLanguageError, docopt.DocoptExit):
         pass
 
 
 class Guards(object):
 
   def __init__(self, script, doc):
@@ -210,15 +210,15 @@
     self.present = self.top.present and self.bottom.present
     # By defaulting start+end to doc.end the parser will be appended to
     # the doc if it is absent
     self.start = self.top.start if self.present else doc.end
     self.end = self.bottom.end if self.present else doc.end
 
   def __len__(self):
-    return self.end - self.start if self.present else 0
+    return self.end - self.start if self.present else 0  # type: ignore
 
 
 class Invocation(ScriptLocation):
 
   def __init__(self, script, parser):
     matches = re.finditer(r'eval "\$\(docopt\s+"\$\@"\)"', script.contents[parser.end:])
     super(Invocation, self).__init__(script, matches, parser.end)
```

### Comparing `docopt-sh-1.0.0/PKG-INFO` & `docopt_sh-2.0.0a1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 Metadata-Version: 2.1
 Name: docopt-sh
-Version: 1.0.0
-Summary: docopt.sh - Bash argument parser generator.
+Version: 2.0.0a1
+Summary: Command-line argument parser for bash 3.2, 4+, and 5+.
 Home-page: https://github.com/andsens/docopt.sh
+License: MIT
 Author: Anders Ingemann
 Author-email: anders@ingemann.de
-Requires-Python: >=3.5
-Description-Content-Type: text/markdown
-Classifier: Topic :: Utilities
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
+Requires-Python: >=3.11.0,<4.0
 Classifier: License :: OSI Approved :: MIT License
-Requires-Dist: docopt
-Requires-Dist: termcolor
-Requires-Dist: pytest ; extra == "test"
-Requires-Dist: pytest-xdist ; extra == "test"
-Requires-Dist: pytest-flake8 ; extra == "test"
-Provides-Extra: test
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Topic :: Utilities
+Requires-Dist: docopt (>=0.6.2,<0.7.0)
+Requires-Dist: docopt-parser (>=0.0.1)
+Requires-Dist: flake8-pyproject (>=1.1.0.post0,<2.0.0)
+Requires-Dist: termcolor (>=1.1.0,<2.0.0)
+Project-URL: Repository, https://github.com/andsens/docopt.sh
+Description-Content-Type: text/markdown
 
 docopt.sh
 =========
 
 A [docopt](http://docopt.org/) argument parser for bash 3.2, 4+, and 5+ with no
 external dependencies.
```

