# Comparing `tmp/pylliterate-0.0.4.tar.gz` & `tmp/pylliterate-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylliterate-0.0.4.tar", max compression
+gzip compressed data, was "pylliterate-0.0.5.tar", max compression
```

## Comparing `pylliterate-0.0.4.tar` & `pylliterate-0.0.5.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1100 2024-05-01 05:46:13.332526 pylliterate-0.0.4/LICENSE
--rw-r--r--   0        0        0    10157 2024-04-25 20:23:18.036017 pylliterate-0.0.4/pylliterate/__init__.py
--rw-r--r--   0        0        0      273 2024-04-24 20:27:28.869868 pylliterate-0.0.4/pylliterate/__main__.py
--rw-r--r--   0        0        0     3817 2024-04-25 20:23:18.036017 pylliterate-0.0.4/pylliterate/cli.py
--rw-r--r--   0        0        0     3145 2024-04-25 20:23:18.038504 pylliterate-0.0.4/pylliterate/config.py
--rw-r--r--   0        0        0    14790 2024-04-25 20:23:18.038504 pylliterate-0.0.4/pylliterate/core.py
--rw-r--r--   0        0        0      665 2024-05-01 05:46:13.333422 pylliterate-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     8544 2024-04-30 05:00:19.884025 pylliterate-0.0.4/Readme.md
--rw-r--r--   0        0        0     9050 1970-01-01 00:00:00.000000 pylliterate-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1100 2024-05-08 21:48:46.550511 pylliterate-0.0.5/LICENSE
+-rw-r--r--   0        0        0    10157 2024-05-10 21:07:14.944125 pylliterate-0.0.5/pylliterate/__init__.py
+-rw-r--r--   0        0        0      273 2024-04-24 20:27:28.869868 pylliterate-0.0.5/pylliterate/__main__.py
+-rw-r--r--   0        0        0     3439 2024-05-10 20:54:10.623176 pylliterate-0.0.5/pylliterate/cli.py
+-rw-r--r--   0        0        0     4135 2024-05-10 21:07:14.959765 pylliterate-0.0.5/pylliterate/config.py
+-rw-r--r--   0        0        0    15018 2024-05-10 21:02:57.167931 pylliterate-0.0.5/pylliterate/core.py
+-rw-r--r--   0        0        0      736 2024-05-10 20:18:17.432177 pylliterate-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     8544 2024-04-30 05:00:19.884025 pylliterate-0.0.5/Readme.md
+-rw-r--r--   0        0        0     9039 1970-01-01 00:00:00.000000 pylliterate-0.0.5/PKG-INFO
```

### Comparing `pylliterate-0.0.4/LICENSE` & `pylliterate-0.0.5/LICENSE`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2020 Jesús Enrique Fuentes
+Copyright (c) 2020 Alejandro Piad Morffis
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pylliterate-0.0.4/pylliterate/__init__.py` & `pylliterate-0.0.5/pylliterate/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -124,27 +124,27 @@
 # that knows how to write itself into a file in Markdown.
 # Note that we just used two internal references in the previous sentences. We'll see how these special constructions
 # are handled when look at the parser implementation but, spoiler alert, it involves some regex.
 # Be aware of the  [`PylliterateConfig`](ref:pylliterate/config:PylliterateConfig) class that hold parameters needed
 # in each processing file
 
 
-def process(input_path: Path, output_path: Path, config: PylliterateConfig):
+def process(input_path: Path, output_path: Path, konfig: PylliterateConfig):
     # We need to create this folder hierarchy if it doesn't exist:
     output_path.parent.mkdir(exist_ok=True)
 
     # First we check if this is just a regular copy
     if input_path.suffix != ".py":
         shutil.copy(input_path, output_path)
         return
 
     # Otherwise, we parse, passing also the file name.
     with input_path.open() as fp:
         content = Parser(
-            fp, config=config, module_name=input_path.name, location=input_path.parent
+            fp, config=konfig, module_name=input_path.name, location=input_path.parent
         ).parse()
 
     # And then we dump the parsed content.
     with output_path.open("w") as fp:
         content.dump(fp)
```

### Comparing `pylliterate-0.0.4/pylliterate/cli.py` & `pylliterate-0.0.5/pylliterate/cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 # !!! info "This module contains the pylliterate CLI application."
 #     The CLI application is basically a [Typer](https://typer.tiangolo.com) application
 #     with three commands, that manage the whole process.
 
-
 # The pylliterate CLI app is a very simple [Typer](https://typer.tiangolo.com)
 # application with three commands.
 # Typer is a CLI creation tool where you define commands as methods,
 # and it takes advantage of Python type annotations to provide argument parsing
 # and documentation.
 
 
 import typer
-import yaml
 
 # These two are for watching file changes.
 
 from watchdog.events import FileModifiedEvent, FileSystemEventHandler
 from watchdog.observers import Observer
 
 # And these are internal.
@@ -27,95 +25,86 @@
 
 from pathlib import Path
 from typing import List
 
 # We start by creating the main typer application and a set of related commands.
 app = typer.Typer()
 
-# ## Command helpers
-
-# Most of the commands will take either CLI args or a --config file. So we will define a private function to take
-# care of configuration load  either from a specified configuration file or using default values and parameters provided
-
-
-def _load_config(src, inline, linenums, highlights, title, config):
-    if config:
-        with config.open() as fp:
-            cfg = PylliterateConfig(**yaml.safe_load(fp))
-    elif not src and Path("pylliterate.yml").exists():
-        with open("pylliterate.yml") as fp:
-            cfg = PylliterateConfig(**yaml.safe_load(fp))
-    else:
-        if not src:
-            typer.echo("At least one source or a config file must be provided.")
-            raise typer.Exit(1)
-        cfg = PylliterateConfig.make(sources=src, inline=inline, linenums=linenums,
-                                     highlights=highlights, title=title)
-    return cfg
 
+# ## Command helpers
 
-# Then we use a decorator to bookkeeping common code between all commands
+# We use a decorator to bookkeeping common code between all commands
 
-def pylliterate_command(fn):
+def configurable(fn):
     def command(
             src: List[str] = typer.Option([]),
             inline: bool = False,
             linenums: bool = False,
             highlights: bool = False,
             title: bool = False,
             config: Path = None,
     ):
-        cfg = _load_config(src, inline, linenums, highlights, title, config)
-        return fn(cfg)
-
+        try:
+            cfg = PylliterateConfig.load(src, inline, linenums, highlights, title, config)
+            return fn(cfg)
+        except PylliterateConfig.ConfigurationNotProvidedException as e:
+            typer.echo(str(e))
+            typer.Exit(code=1)
     return command
 
 
 # ## The build command
 
 # Here is the implementation of the build command
 # is called when `python -m pylliterate build` is used.
 # This command parse and creates the documentation based on its input parameters.
 
 
 @app.command("build")
-@pylliterate_command
+@configurable
 def build(config: PylliterateConfig):
     process_all(config)
 
 
 # ## The config command
-
+#
+# > we named it konfig to avoid clashes with config parameter and shadowing
 
 @app.command("config")
-@pylliterate_command
-def config(config: PylliterateConfig):
-    print(yaml.safe_dump(config.dict()))
+@configurable
+def konfig(config: PylliterateConfig):
+    print(config)
 
 
-class IlliterateHandler(FileSystemEventHandler):
+# ## The watching system
+#
+# With `watchdog` we need to define a class that hold the logic to be executed when filesystem change
+# the PylliterateHandler class fulfil that purpose
+class PylliterateHandler(FileSystemEventHandler):
     def __init__(
             self, input_path: Path, output_path: Path, cfg: PylliterateConfig
     ) -> None:
         super().__init__()
         self.cfg = cfg
         self.input_path = input_path
         self.output_path = output_path
 
     def on_modified(self, event: FileModifiedEvent):
         typer.echo(f"Recreating: {self.input_path} -> {self.output_path}")
         process(self.input_path, self.output_path, self.cfg)
 
 
+# Then we add a command (maybe a flag in the needed command is just a better idea) that set up the watchdog observer
+# mechanism over filesystem using our handler
 @app.command("watch")
-@pylliterate_command
+@configurable
 def watch(config: PylliterateConfig):
     process_all(config)
     observer = Observer()
 
     for input_path, output_path in config.files:
         observer.schedule(
-            IlliterateHandler(input_path, output_path, config), input_path
+            PylliterateHandler(input_path, output_path, config), input_path
         )
 
     observer.start()
     observer.join()
```

### Comparing `pylliterate-0.0.4/pylliterate/config.py` & `pylliterate-0.0.5/pylliterate/config.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,24 +3,28 @@
 
 
 # We start as usually,  importing necessary modules
 
 import logging
 from functools import cached_property
 from pathlib import Path
-from typing import Dict, List
+import yaml
+from typing import Dict
 from pydantic import BaseModel
 
 logger = logging.getLogger("pylliterate")
 
+
 # ## The configuration class
-# We define a configuration class for Pylliterate using Pydantic's BaseModel for proper auto mapping and validation
+#
+# We define a configuration class for Pylliterate using Pydantic BaseModel for proper
+# auto mapping and validation. We took a KISS and single responsibility approach binding all configuration related
+# logic to this class instead of build an anemic POJO class
 
 class PylliterateConfig(BaseModel):
-
     # 'inline' specifies if the documentation is shown inline within the source code
     inline: bool = False
 
     # 'title' specifies if headings/titles should be created in the documentation
     title: bool = False
 
     # 'linenums' specifies if line numbers should be included in the documentation
@@ -28,44 +32,64 @@
 
     # 'highlights' specifies if code snippets should be highlighted
     highlights: bool = False
 
     # sources is a dictionary mapping source file paths to their respective documentation file paths
     sources: Dict[str, str]
 
+    # A class error bound to this class because `only this class can throw that error`, is the error threw when
+    # pylliterate configuration isn't provided
+
+    class ConfigurationNotProvidedException(Exception):
+        def __init__(self):
+            super().__init__("At least one source or a config file must be provided.")
+
     # We need a class method that creates an instance of PylliterateConfig
     # from a list of source files and other options, the make method fulfill goal
     @classmethod
-    def make(cls, *, sources: List[str], **kwargs):
-        # initialize empty dictionary
-        source_dict = {}
-
-        # iterate over every source line
-        for line in sources:
-            # split the line into the input file path and output file path
-            input, output = line.split(":")
-            # add the input and output paths to the dictionary
-            source_dict[input] = output
-
-        # return an instance of PylliterateConfig with the specified sources and options
-        return cls(sources=source_dict, **kwargs)
+    def load(cls, src, inline, linenums, highlights, title, config) -> "PylliterateConfig":
+        if config:
+            with config.open() as fp:
+                cfg = cls(**yaml.safe_load(fp))
+        elif not src and Path("pylliterate.yml").exists():
+            with open("pylliterate.yml") as fp:
+                cfg = cls(**yaml.safe_load(fp))
+        else:
+            if not src:
+                raise cls.ConfigurationNotProvidedException()
+            sources = {}
+
+            # iterate over every source line
+            for line in src:
+                # split the line into the input file path and output file path
+                i, o = line.split(":")
+                # add the input and output paths to the dictionary
+                sources[i] = o
+
+            # return an instance of PylliterateConfig with the specified sources and options
+            cfg = cls(sources=sources, inline=inline, linenums=linenums,
+                      highlights=highlights, title=title)
+        return cfg
 
     # Since the sources attribute is a user-friendly representation of the file system,
     # we need to process it in order to use it correctly. That's what the property files does.
 
     @cached_property
     def files(self):
         # iterate over all items (input and output paths) in the sources dictionary
         for input_path, output_path in self.sources.items():
             # yield a tuple of Path objects for the input source file and its corresponding documentation file
             in_path, out_path = Path(input_path).resolve(), Path(output_path).resolve()
 
             # if the input path if a directory we try to expand it
             if in_path.is_dir() and out_path.is_dir():
                 for file in in_path.rglob("*.py"):
-                    yield (in_path / file.relative_to(in_path)), (out_path / in_path.relative_to(Path.cwd()) / str(file.relative_to(in_path))
-                                                                  .replace(".py", ".md"))
+                    yield (in_path / file.relative_to(in_path)), (
+                            out_path / in_path.relative_to(Path.cwd()) / str(file.relative_to(in_path))
+                            .replace(".py", ".md"))
             elif in_path.is_file():
-                print(in_path, out_path)
                 yield in_path, out_path
             else:
                 logger.warning(f"Improper input or output path for {in_path} and {out_path}.")
+
+    def __str__(self):
+        return yaml.safe_dump(self.dict())
```

### Comparing `pylliterate-0.0.4/pylliterate/core.py` & `pylliterate-0.0.5/pylliterate/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,19 @@
 
 from __future__ import annotations
 
 import logging
 import collections
 from pathlib import Path
 
+import abc
+import re
+import enum
+from typing import TextIO, List
+
 from pylliterate.config import PylliterateConfig
 
 logger = logging.getLogger("pylliterate")
 
 # To represent the different types of content in a single Python file,
 # we will use three classes.
 # These classes will represent, respectively,
@@ -29,20 +34,14 @@
 # This might not be a big issue for Markdown, in some cases, but it is
 # definitely a problem for Python code.
 # Hence, we will remove all the empty lines at the beginning and the end
 # of each block.
 
 # The common functionality will go into an abstract class.
 
-import abc
-import re
-import enum
-from typing import TextIO, List
-
-
 # ## Content Blocks
 
 # The only relevant functionality in this class is cleaning up
 # the list of content.
 # We also define an abstract method `print` which inheritors
 # will override to determine how different types of content are printed.
 
@@ -50,21 +49,21 @@
 class Block(abc.ABC):
     def __init__(self, name: str, content: List[str], module_name: str, lineno: int):
         self.module_name = module_name
         self.lineno = lineno
         self.name = name
 
         while content:
-            if not content[0].strip():  # testing for emptyness
+            if not content[0].strip():  # testing for emptiness
                 content.pop(0)  # from the top down
             else:
                 break
 
         while content:
-            if not content[-1].strip():  # testing for emptyness
+            if not content[-1].strip():  # testing for emptiness
                 content.pop()  # from the bottom up
             else:
                 break
 
         self.content = content
 
     def __str__(self):
@@ -94,29 +93,32 @@
     hl_re = re.compile(r":hl:(?P<ref>[a-zA-Z0-9_]+):")
     include_re = re.compile(r":include:((?P<start>-?\d+):)?((?P<end>-?\d+):)?(?P<file>.*):")
 
     def print(self, fp: TextIO, content: Content):
         for line in self.content:
             line = self.fix_links(line.strip())
 
-            if line.startswith("# "):
+            # Ignoring inspection disabling lines for Intellij IDE
+            if line.find("noinspection") != -1:
+                continue
+            elif line.startswith("# "):
                 if match := self.hl_re.search(line):
                     ref = match.group("ref")
                     block = content[ref]
                     block.print(fp, content)
                     continue
 
                 if match := self.include_re.search(line):
                     start = int(match.group('start') or 0) - 1
                     end = int(match.group('end') or -1)
                     file = match.group('file')
 
                     with open(content.location / file) as include:
                         lines = include.readlines()
-
+                        # noinspection PyAssignmentToLoopOrWithParameter
                         for line in lines[start:end]:
                             fp.write(line)
                     continue
 
                 fp.write(line[2:] + "\n")
             else:
                 fp.write("\n")
@@ -212,15 +214,16 @@
 
             if match:
                 anchors.append(f"<a name=\"ref:{match.group('name')}\"></a>")
                 logger.debug("Found anchor: %r" % match)
 
         return anchors
 
-    def strip(self, line: str):
+    @staticmethod
+    def strip(line: str):
         result = []
         comment = False
 
         for c in line:
             if c == "#":
                 comment = True
```

### Comparing `pylliterate-0.0.4/pyproject.toml` & `pylliterate-0.0.5/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 [tool.poetry]
 name = "pylliterate"
-version = "0.0.4"
+version = "0.0.5"
 description = "Unobtrusive literate programming experience for Python pragmatists"
-authors = ["Jesús Enrique Fuentes <jesusefg12@gmail.com>", "Alejandro Piad <alepiad@gmail.com>"]
+# Poetry is ignoring multiple autors configuration line but's ok :)
+authors = ["Alejandro Piad <alepiad@gmail.com>", "Jesús Enrique Fuentes <jesusefg12@gmail.com>"]
+
 license = "MIT"
 readme = "Readme.md"
 
 [tool.poetry.scripts]
 pylliterate = "pylliterate.cli:app"
 
 [tool.poetry.dependencies]
```

### Comparing `pylliterate-0.0.4/Readme.md` & `pylliterate-0.0.5/Readme.md`

 * *Files identical despite different names*

### Comparing `pylliterate-0.0.4/PKG-INFO` & `pylliterate-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: pylliterate
-Version: 0.0.4
+Version: 0.0.5
 Summary: Unobtrusive literate programming experience for Python pragmatists
 License: MIT
-Author: Jesús Enrique Fuentes
-Author-email: jesusefg12@gmail.com
+Author: Alejandro Piad
+Author-email: alepiad@gmail.com
 Requires-Python: >=3.12,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: PyYAML (>=6.0.1,<7.0.0)
 Requires-Dist: pydantic (>=2.7.1,<3.0.0)
 Requires-Dist: rich (>=9.0.1,<10.0.0)
```

