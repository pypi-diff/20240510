# Comparing `tmp/exsource_tools-0.0.5.tar.gz` & `tmp/exsource_tools-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exsource_tools-0.0.5.tar", last modified: Fri Oct 27 14:34:19 2023, max compression
+gzip compressed data, was "exsource_tools-0.0.6.tar", last modified: Fri May 10 14:58:49 2024, max compression
```

## Comparing `exsource_tools-0.0.5.tar` & `exsource_tools-0.0.6.tar`

### file list

```diff
@@ -1,25 +1,27 @@
-drwxrwxr-x   0 js3214    (1000) js3214    (1000)        0 2023-10-27 14:34:19.242435 exsource_tools-0.0.5/
--rw-rw-r--   0 js3214    (1000) js3214    (1000)    42098 2023-04-17 21:22:16.000000 exsource_tools-0.0.5/LICENSE
--rw-r--r--   0 js3214    (1000) js3214    (1000)     1423 2023-10-27 14:34:19.242435 exsource_tools-0.0.5/PKG-INFO
--rw-rw-r--   0 js3214    (1000) js3214    (1000)      546 2023-04-17 21:16:27.000000 exsource_tools-0.0.5/README.md
-drwxrwxr-x   0 js3214    (1000) js3214    (1000)        0 2023-10-27 14:34:19.238435 exsource_tools-0.0.5/exsource_tools/
--rw-rw-r--   0 js3214    (1000) js3214    (1000)      170 2023-10-16 16:02:26.000000 exsource_tools-0.0.5/exsource_tools/__init__.py
--rw-rw-r--   0 js3214    (1000) js3214    (1000)     3447 2023-10-16 15:48:47.000000 exsource_tools-0.0.5/exsource_tools/cli.py
--rw-rw-r--   0 js3214    (1000) js3214    (1000)    14488 2023-10-27 12:21:16.000000 exsource_tools-0.0.5/exsource_tools/exsource.py
-drwxrwxr-x   0 js3214    (1000) js3214    (1000)        0 2023-10-27 14:34:19.242435 exsource_tools-0.0.5/exsource_tools/schemas/
--rw-rw-r--   0 js3214    (1000) js3214    (1000)     5044 2023-05-03 14:26:55.000000 exsource_tools-0.0.5/exsource_tools/schemas/exsource.schema.json
--rw-rw-r--   0 js3214    (1000) js3214    (1000)    12077 2023-10-27 12:19:30.000000 exsource_tools-0.0.5/exsource_tools/tools.py
--rw-rw-r--   0 js3214    (1000) js3214    (1000)     4683 2023-10-23 14:52:27.000000 exsource_tools-0.0.5/exsource_tools/utils.py
-drwxrwxr-x   0 js3214    (1000) js3214    (1000)        0 2023-10-27 14:34:19.242435 exsource_tools-0.0.5/exsource_tools.egg-info/
--rw-r--r--   0 js3214    (1000) js3214    (1000)     1423 2023-10-27 14:34:19.000000 exsource_tools-0.0.5/exsource_tools.egg-info/PKG-INFO
--rw-rw-r--   0 js3214    (1000) js3214    (1000)      502 2023-10-27 14:34:19.000000 exsource_tools-0.0.5/exsource_tools.egg-info/SOURCES.txt
--rw-rw-r--   0 js3214    (1000) js3214    (1000)        1 2023-10-27 14:34:19.000000 exsource_tools-0.0.5/exsource_tools.egg-info/dependency_links.txt
--rw-rw-r--   0 js3214    (1000) js3214    (1000)      100 2023-10-27 14:34:19.000000 exsource_tools-0.0.5/exsource_tools.egg-info/entry_points.txt
--rw-rw-r--   0 js3214    (1000) js3214    (1000)        1 2023-04-17 12:35:00.000000 exsource_tools-0.0.5/exsource_tools.egg-info/not-zip-safe
--rw-rw-r--   0 js3214    (1000) js3214    (1000)       52 2023-10-27 14:34:19.000000 exsource_tools-0.0.5/exsource_tools.egg-info/requires.txt
--rw-rw-r--   0 js3214    (1000) js3214    (1000)       21 2023-10-27 14:34:19.000000 exsource_tools-0.0.5/exsource_tools.egg-info/top_level.txt
--rw-rw-r--   0 js3214    (1000) js3214    (1000)       38 2023-10-27 14:34:19.242435 exsource_tools-0.0.5/setup.cfg
--rw-rw-r--   0 js3214    (1000) js3214    (1000)     2170 2023-10-27 14:27:25.000000 exsource_tools-0.0.5/setup.py
-drwxrwxr-x   0 js3214    (1000) js3214    (1000)        0 2023-10-27 14:34:19.242435 exsource_tools-0.0.5/tests/
--rw-rw-r--   0 js3214    (1000) js3214    (1000)        0 2023-04-21 09:39:47.000000 exsource_tools-0.0.5/tests/__init__.py
--rw-rw-r--   0 js3214    (1000) js3214    (1000)     2327 2023-10-16 16:04:06.000000 exsource_tools-0.0.5/tests/test_exsource.py
+drwxrwxr-x   0 js3214    (1000) js3214    (1000)        0 2024-05-10 14:58:49.142028 exsource_tools-0.0.6/
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)    42098 2023-04-17 21:22:16.000000 exsource_tools-0.0.6/LICENSE
+-rw-r--r--   0 js3214    (1000) js3214    (1000)     2240 2024-05-10 14:58:49.138028 exsource_tools-0.0.6/PKG-INFO
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)     1323 2024-02-14 14:15:26.000000 exsource_tools-0.0.6/README.md
+drwxrwxr-x   0 js3214    (1000) js3214    (1000)        0 2024-05-10 14:58:49.138028 exsource_tools-0.0.6/exsource_tools/
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)      233 2024-02-08 11:31:14.000000 exsource_tools-0.0.6/exsource_tools/__init__.py
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)     3447 2023-10-16 15:48:47.000000 exsource_tools-0.0.6/exsource_tools/cli.py
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)      525 2024-02-08 11:13:13.000000 exsource_tools-0.0.6/exsource_tools/enums.py
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)    13144 2024-02-14 14:06:05.000000 exsource_tools-0.0.6/exsource_tools/exporters.py
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)    14558 2024-02-14 14:06:05.000000 exsource_tools-0.0.6/exsource_tools/exsource.py
+drwxrwxr-x   0 js3214    (1000) js3214    (1000)        0 2024-05-10 14:58:49.138028 exsource_tools-0.0.6/exsource_tools/schemas/
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)     5044 2023-05-03 14:26:55.000000 exsource_tools-0.0.6/exsource_tools/schemas/exsource.schema.json
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)     8022 2024-02-08 15:20:10.000000 exsource_tools-0.0.6/exsource_tools/tools.py
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)     4683 2024-02-07 17:44:45.000000 exsource_tools-0.0.6/exsource_tools/utils.py
+drwxrwxr-x   0 js3214    (1000) js3214    (1000)        0 2024-05-10 14:58:49.138028 exsource_tools-0.0.6/exsource_tools.egg-info/
+-rw-r--r--   0 js3214    (1000) js3214    (1000)     2240 2024-05-10 14:58:49.000000 exsource_tools-0.0.6/exsource_tools.egg-info/PKG-INFO
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)      554 2024-05-10 14:58:49.000000 exsource_tools-0.0.6/exsource_tools.egg-info/SOURCES.txt
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)        1 2024-05-10 14:58:49.000000 exsource_tools-0.0.6/exsource_tools.egg-info/dependency_links.txt
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)      100 2024-05-10 14:58:49.000000 exsource_tools-0.0.6/exsource_tools.egg-info/entry_points.txt
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)        1 2023-04-17 12:35:00.000000 exsource_tools-0.0.6/exsource_tools.egg-info/not-zip-safe
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)       61 2024-05-10 14:58:49.000000 exsource_tools-0.0.6/exsource_tools.egg-info/requires.txt
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)       21 2024-05-10 14:58:49.000000 exsource_tools-0.0.6/exsource_tools.egg-info/top_level.txt
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)       38 2024-05-10 14:58:49.142028 exsource_tools-0.0.6/setup.cfg
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)     2182 2024-02-14 14:17:13.000000 exsource_tools-0.0.6/setup.py
+drwxrwxr-x   0 js3214    (1000) js3214    (1000)        0 2024-05-10 14:58:49.138028 exsource_tools-0.0.6/tests/
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)        0 2023-04-21 09:39:47.000000 exsource_tools-0.0.6/tests/__init__.py
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)     3811 2024-02-14 14:06:05.000000 exsource_tools-0.0.6/tests/test_exsource.py
```

### Comparing `exsource_tools-0.0.5/LICENSE` & `exsource_tools-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `exsource_tools-0.0.5/PKG-INFO` & `exsource_tools-0.0.6/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: exsource_tools
-Version: 0.0.5
+Version: 0.0.6
 Summary: Python tools for using Exsource files
 Home-page: https://gitlab.com/gitbuilding/exsource-tools
 Author: Julian Stirling
 Author-email: julian@julianstirling.co.uk
 License: LGPLv3
 Project-URL: Bug Tracker, https://gitlab.com/gitbuilding/exsource-tools/issues
 Project-URL: Source Code, https://gitlab.com/gitbuilding/exsource-tools
@@ -17,17 +17,50 @@
 License-File: LICENSE
 Requires-Dist: argparse
 Requires-Dist: pyyaml>=5.1
 Requires-Dist: jsonschema
 Provides-Extra: dev
 Requires-Dist: pylint; extra == "dev"
 Requires-Dist: twine; extra == "dev"
+Requires-Dist: colorama; extra == "dev"
 
 # ExSource-Tools
 
 An experimental Python library for validating and using the [ExSource Specification](https://gitlab.com/gitbuilding/exsourcespec) which is in the early stage of development.
 
+## Commands
+
+### Make
+
 This packages adds the following command:
 
-    exsource-make exsource.yml
+    exsource-make
+
+This will attempt to process `exsource-def.yml` to create inputs. The first instance of this proof of principle implementation supports OpenSCAD, FreeCAD, and CadQuery files. Each of these must be installed separately if they are to be used.
+
+***FreeCAD***  
+By default FreeCAD exporter will expect there to be a PartDesign Body called `Body`, it can export this to STEP and/or STL. The body to export can be changed by specifying the label of the object with `object-selected` as a parameter. For example:
+```yaml
+frame:
+    name: Main frame
+    description: >
+        This frame holds the shelf brackets and shelves.
+    output-files:
+        - output/frame.step
+        - output/frame.stl
+    source-files:
+        - assets/frame.FCStd
+    parameters:
+        object-selected: "Frame"
+    application: freecad
+```
+
+***CadQuery***  
+The CardQuery export is performed via [cq-cli](https://github.com/CadQuery/cq-cli)
+
+### Check
+
+You can also use the command:
+
+    exsource-check
 
-This will attempt to process `exsource.yml` to create inputs. The first instance of this proof of principle implementation supports OpenSCAD and some FreeCAD files. FreeCAD exporter will expect there to be a PartDesign Body called `Body`, it can export this to STEP and/or STL.
+This will specify what would happen if `exsource-make` was run.
```

### Comparing `exsource_tools-0.0.5/exsource_tools/cli.py` & `exsource_tools-0.0.6/exsource_tools/cli.py`

 * *Files identical despite different names*

### Comparing `exsource_tools-0.0.5/exsource_tools/exsource.py` & `exsource_tools-0.0.6/exsource_tools/exsource.py`

 * *Files 0% similar despite different names*

```diff
@@ -80,15 +80,16 @@
         with open(schema_file, 'r', encoding="utf-8") as file_obj:
             schema = json.loads(file_obj.read())
         return schema
 
     @property
     def exports(self):
         """
-        Return the list of ExSourceExport objects
+        Return the dictionary of each key is the export name (id),
+        the values are ExSourceExport objects
         """
         return self._exports
 
     @property
     def all_output_files(self):
         """
         A list of output files for every export combined
@@ -385,15 +386,15 @@
         if isinstance(other, str):
             return self.filepath == other
         if isinstance(other, ExSourceFile):
             if self.md5 is None or self.md5 == other.md5:
                 if self.filepath == other.filepath:
                     return True
             return False
-        super().__eq__(other)
+        return super().__eq__(other)
 
     def __repr__(self):
         return self._filepath
 
     def dump(self):
         """
         Return the data for this file as a python dictionary.
```

### Comparing `exsource_tools-0.0.5/exsource_tools/schemas/exsource.schema.json` & `exsource_tools-0.0.6/exsource_tools/schemas/exsource.schema.json`

 * *Files identical despite different names*

### Comparing `exsource_tools-0.0.5/exsource_tools/tools.py` & `exsource_tools-0.0.6/exsource_tools/exporters.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,290 +1,366 @@
 """
-Tools for processing ExSourceFiles.
+Classes for exporting hardware files
 """
 from os import path
-import json
 import subprocess
-from copy import deepcopy
-from tempfile import gettempdir
 import logging
-import yaml
+from tempfile import gettempdir
 
 from exsource_tools import utils
-from exsource_tools.exsource import ExSource
+from exsource_tools.enums import Status
 
 logging.basicConfig()
 LOGGER = logging.getLogger('exsource')
 LOGGER.setLevel(logging.INFO)
 
+class BaseExporter:
+    """
+    This is a base class for exporters. Don't try to run this class
+    The exporter runs one "export" from the exsorce. It will export
+    all output files. Input to init is one ExSourceExport object.
+    """
 
+    name = "Base"
+    executable = None
+    min_outputs = 1
+    max_outputs = None
+    min_sources = 1
+    max_sources = None
 
-UNSTAGED = 0
-PENDING = 1
-SKIPPED = 2
-PROCESSED = 3
-
-CONTINUE = 10
-SKIP = 11
-DELAY = 12
-UNCHANGED = 13
-UNCHANGED_INCOMPLETE = 14
-CHANGED = 15
-NEW = 16
-DETAILS_CHANGED = 17
-DETAILS_CHANGED_INCOMPLETE = 18
+    def __init__(self, export, headless=False):
+        self.export = export
+        self.headless = headless
 
+    @property
+    def output_files(self):
+        """
+        Property shorthand returning all output files as a list of
+        ExSourceFile objects
+        """
+        return self.export.output_files
 
-def load_exsource_file(filepath):
-    """
-    Load an exsource file from the inupt filepath. An ExSource object is returned
-    """
-    file_format = utils.exsource_file_format(filepath, "read")
-    with open(filepath, 'r', encoding="utf-8") as file_obj:
-        file_content = file_obj.read()
-        if file_format == "JSON":
-            input_data = json.loads(file_content)
-        else:
-            #only other option is YAML
-            input_data = yaml.safe_load(file_content)
-    return ExSource(input_data)
+    @property
+    def source_files(self):
+        """
+        Property shorthand returning all source files as a list of
+        ExSourceFile objects
+        """
+        return self.export.source_files
 
-class ExSourceProcessor:
-    """
-    This class processes the data in the exsource file to create all the ouputs.
-    Currently it only works for certain OpenSCAD and FreeCAD exports
-    """
+    @property
+    def outputs_valid(self):
+        """
+        Check if there are the expected number of outputs. Return True if valid
+        """
+        if len(self.output_files) < self.min_outputs:
+            LOGGER.warning("%s expects a minimum of %d outputs to be specified",
+                           self.name, self.min_outputs)
+            return False
+        if self.max_outputs is not None:
+            if len(self.output_files) > self.max_outputs:
+                LOGGER.warning("%s expects a maximum of %d outputs to be specified",
+                               self.name, self.min_outputs)
+                return False
+        return True
 
-    def __init__(self,
-                 exsource_def,
-                 previous_exsource=None,
-                 exsource_out_path=None,
-                 headless=False):
+    @property
+    def sources_valid(self):
+        """
+        Check if there are the expected number of sources. Check sources exist
+        on disk. Return True if valid
+        """
+        if len(self.source_files) < self.min_sources:
+            LOGGER.warning("%s expects a minimum of %d sources to be specified",
+                           self.name, self.min_sources)
+            return False
+        if self.max_sources is not None:
+            if len(self.source_files) > self.max_sources:
+                LOGGER.warning("%s expects a maximum of %d sources to be specified",
+                               self.name, self.min_sources)
+                return False
+        for source in self.source_files:
+            if not path.exists(source.filepath):
+                LOGGER.warning("Source file %s does not exist, skipping.",
+                               source.filepath)
+                return False
+        return True
 
-        self.headless = headless
-        self._exsource = deepcopy(exsource_def)
-        self._exsource_prev = previous_exsource
-        self._exsource_out_path = exsource_out_path
-        self._all_output_files = {output.filepath: UNSTAGED for output in self._exsource.all_output_files}
-
-    def check(self, echo=True):
-        """
-        Check which files require exporting
-        """
-        if self._exsource_prev is None:
-            if echo:
-                print("No exsource-out found.")
-            return {export_id: NEW for export_id in self._exsource.exports.items()}
-
-        output = {}
-        for export_id, export in self._exsource.exports.items():
-            output[export_id] = self._check_dependencies(export_id, export)
-
-            if echo:
-                if output[export_id] == NEW:
-                    print(f"Export {export_id} not in previous run.")
-                elif output[export_id] == UNCHANGED:
-                    print(f"Export {export_id}: is unchanged, no processing needed")
-                elif output[export_id] == UNCHANGED_INCOMPLETE:
-                    print(f"Export {export_id}: is unchanged, however not all dependencies are known")
-                elif output[export_id] == DETAILS_CHANGED:
-                    print(f"Export {export_id}: outputs are unchanged, details have been updated")
-                elif output[export_id] == DETAILS_CHANGED_INCOMPLETE:
-                    print(f"Export {export_id}:  outputs are unchanged, details have been updated and not all dependencies are known")
-                else:
-                    print(f"Export {export_id}: has changed, any ouput files need regenerating.")
-        return output
-
-    def make(self):
-        """
-        Process all exsource exports (if possible)
-        """
-        self._all_output_files = {output.filepath: PENDING for output in self._exsource.all_output_files}
-        iteration = 0
-        unprocessed_exports = self._exsource.exports
-        while len(unprocessed_exports) > 0:
-            #TODO: make less simplistic
-            iteration += 1
-            if iteration > len(self._exsource.exports):
-                raise RuntimeError("Circular dependencies in exsource file")
-
-            unprocessed_exports = self._process_exports(unprocessed_exports)
-
-        outpath = self._exsource_out_path
-        if outpath is None:
-            outpath = 'exsource-out.yml'
-        self._exsource.save(outpath)
-
-    def _process_exports(self, exports_to_process):
-        unprocessed_exports = {}
-
-        for export_id, export in exports_to_process.items():
-            LOGGER.info("Processing export: %s", export_id)
-            app = export.application
-
-            dep_status = self._check_dependencies(export_id, export)
-            if dep_status in [UNCHANGED, DETAILS_CHANGED]:
-                LOGGER.info("Export %s: is unchanged, no processing needed", export_id)
-                #Move all extra information over if eveything is unchanged since last run.
-                # Updated details are coppied over without re running files
-                new_export = deepcopy(self._exsource_prev.exports[export_id])
-                new_export.name = export.name
-                new_export.description = export.description
-                self._exsource.exports[export_id] = new_export
-                continue
+    def x_required(self, output): #pylint: disable=unused-argument
+        """
+        Return true if an X server is required to create this output. This will
+        use xvfb-run to run the command if exsource has been run in headless mode.
+        """
+        return False
+
+    @property
+    def parameter_agruments(self):
+        """
+        Not implemented in this class. Child classes should reimplement this
+        to return a list of arguments to be passed into the subprocess call
+        """
+        raise NotImplementedError
 
-            #If the dependncy was changed. Decide the action and proceed.
-            action = self._decide_action(export)
+    def file_arguments(self, output):
+        """
+        Not implemented in this class. Child classes should reimplement this
+        to return a list of file arguments to be passed into the subprocess call
+        """
+        raise NotImplementedError
+
+    @property
+    def option_arguments(self):
+        """
+        Splits up the application options into a list for the subprocess call
+        """
+        return utils.split_app_options(self.export.app_options)
+
+    def handle_dependencies(self, output): #pylint: disable=unused-argument
+        """
+        If the exporter can automatically track dependencies to be added to the
+        exsource-out file then this tracking should be implemented in this class
+        """
+
+    def print_output_on_success(self, ret):
+        """
+        Print to console the output from a successful output generation
+        """
+        std_out = ret.stdout.decode('UTF-8')
+        print(std_out)
+
+    def output_str_from_error(self, err):
+        """
+        Return the text output from a successful output generation
+        """
+        std_out = err.stdout.decode('UTF-8')
+        std_err = err.stderr.decode('UTF-8')
+        return f"{std_out}\n{std_err}"
+
+    def check_return_for_hidden_error(self, ret, output):  #pylint: disable=unused-argument
+        """
+        Not implemented in the base class. This can be used to check what is returned
+        from a program call to check for errors as not every program sets a non-zero
+        error code on failure.
+        """
+
+    def run_executable(self, output, require_x):
+        """
+        Run the executable to generate the output.
+        """
+        params = self.parameter_agruments
+        file_args = self.file_arguments(output)
+        options = self.option_arguments
+
+        all_args = options + params + file_args
 
-            if action == CONTINUE:
-                if app.lower() == "openscad":
-                    self._process_openscad(export)
-                elif app.lower() == "freecad":
-                    self._process_freecad(export)
-                else:
-                    LOGGER.warning("Skipping %s as no methods available process files with %s",
-                                   export_id,
-                                   app)
-                    for output in export.output_files:
-                        self._all_output_files[output.filepath] = SKIPPED
-            elif action == SKIP:
-                for output in export.output_files:
-                    self._all_output_files[output.filepath] = SKIPPED
-                LOGGER.warning("Skipping %s it has skipped dependencies", export_id)
-            elif action == DELAY:
-                unprocessed_exports[export_id] = export
-                LOGGER.info("Delaying %s as it has unprocessed dependencies", export_id)
-
-        return unprocessed_exports
-
-    def _check_dependencies(self, export_id, export):
-        """
-        Check if files need processing based on dependency and source file status
-        """
-
-        if self._exsource_prev is None:
-            return NEW
-
-        if export_id not in self._exsource_prev.exports:
-            return NEW
-
-        prev_export = self._exsource_prev.exports[export_id]
-        if export.unchanged_from(prev_export):
-            exhaustive = prev_export.dependencies_exhaustive
-            if export.details_unchanged_from(prev_export):
-                unchanged_status = UNCHANGED if exhaustive else UNCHANGED_INCOMPLETE
+        try:
+            if self.headless and require_x:
+                xrvb_args = ['xvfb-run',
+                            '--auto-servernum',
+                            '--server-args',
+                            '-screen 0 1024x768x24']
+                args = xrvb_args + [self.executable] + all_args
             else:
-                unchanged_status = DETAILS_CHANGED if exhaustive else DETAILS_CHANGED_INCOMPLETE
-            return unchanged_status
-        return CHANGED
-
-    def _decide_action(self, export):
-        """
-        action to take based on dependency file status
-        """
-        action = CONTINUE
-        for dep in export.dependencies + export.source_files:
-            dep.store_hash()
-            if dep.filepath in self._all_output_files:
-                dep_status = self._all_output_files[dep.filepath]
-                if dep_status == SKIPPED:
-                    return SKIP
-                if dep_status == PENDING:
-                    LOGGER.info("Dependent file: %s not yet processed", dep.filepath)
-                    action = DELAY
-                    #No return here as another dependency might require it to be skipped
-
-        return action
-
-    def _process_openscad(self, export):
-        #TODO: Tidy up
-        assert len(export.output_files) == 1, "OpenSCAD expects only one output"
-        output = export.output_files[0]
-        assert len(export.source_files) == 1, "Openscad expects only one source file"
-        source = export.source_files[0]
+                args = [self.executable] + all_args
+            ret = subprocess.run(args, check=True, capture_output=True)
+            self.print_output_on_success(ret)
+            self.check_return_for_hidden_error(ret, output)
+        except subprocess.CalledProcessError as err:
+            out_str = self.output_str_from_error(err)
+            raise RuntimeError(f"\n\n{self.name} failed create file: {output.filepath}"
+                               f" with error:\n\n{out_str}") from err
+
+    def process_export(self, output_file_statuses):
+        """
+        This is the what should be called after initalisation to generate the ouput file
+        """
+        valid = self.outputs_valid and self.sources_valid
+
+        if not valid:
+            for output in self.output_files:
+                output_file_statuses[output.filepath] = Status.SKIPPED
+            return
+
+        for output in self.output_files:
+            utils.add_directory_if_needed(output.filepath)
+            require_x = self.x_required(output)
+            self.run_executable(output, require_x)
+            output.store_hash()
+            self.handle_dependencies(output)
+            output_file_statuses[output.filepath] = Status.PROCESSED
+
 
-        require_x = True if output.filepath.lower().endswith('.png') else False
+class OpenSCADExporter(BaseExporter):
+    """
+    This is a exporter class for OpenSCAD.
+    """
+
+    name = "OpenSCAD"
+    executable = "openscad"
+    min_outputs = 1
+    max_outputs = 1
+    min_sources = 1
+    max_sources = 1
 
+    def x_required(self, output): #pylint: disable=unused-argument
+        """
+        Set that an x-server is required if this output is a PNG
+        """
+        return output.filepath.lower().endswith('.png')
 
+    @property
+    def parameter_agruments(self):
+        """
+        Parse the parameters into a list of the command line arguments to be used
+        for the subprocess call
+        """
         params = []
-        for parameter in export.parameters:
-            if isinstance(export.parameters[parameter], (float, int)):
-                par = str(export.parameters[parameter])
-            elif isinstance(export.parameters[parameter], bool):
+        for parameter in self.export.parameters:
+            if isinstance(self.export.parameters[parameter], (float, int)):
+                par = str(self.export.parameters[parameter])
+            elif isinstance(self.export.parameters[parameter], bool):
                 #ensure lowercase for booleans
-                par = str(export.parameters[parameter]).lower()
-            elif isinstance(export.parameters[parameter], str):
-                par = export.parameters[parameter]
+                par = str(self.export.parameters[parameter]).lower()
+            elif isinstance(self.export.parameters[parameter], str):
+                par = self.export.parameters[parameter]
             else:
                 LOGGER.warning("Can only process string, numerical or boolean arguments "
                                "for OpenSCAD. Skipping parameter %s", parameter)
                 continue
             params.append("-D")
             params.append(f"{parameter}={par}")
+        return params
 
-        executable = "openscad"
+    def depfilename(self, output):
+        """
+        Return the depfilename for the specified output
+        """
+        return output.filepath + ".d"
 
-        depfilename = output.filepath + ".d"
-        utils.add_directory_if_needed(output.filepath)
-        openscad_file_args = ["-d", depfilename, "-o", output.filepath, source.filepath]
-        options = utils.split_app_options(export.app_options)
-        openscad_args = options + params + openscad_file_args
-        try:
-            if self.headless and require_x:
-                xrvb_args = ['xvfb-run',
-                             '--auto-servernum',
-                             '--server-args',
-                             '-screen 0 1024x768x24']
-                args = xrvb_args + [executable] + openscad_args
-            else:
-                args = [executable] + openscad_args
-            ret = subprocess.run(args, check=True, capture_output=True)
-            #print std_err as OpenSCAD uses it to print rather than std_out
-            std_err = ret.stderr.decode('UTF-8')
-            print(std_err)
-        except subprocess.CalledProcessError as error:
-            std_err = error.stderr.decode('UTF-8')
-            raise RuntimeError(f"\n\nOpenSCAD failed create file: {output} with error:\n\n"
-                               f"{std_err}") from error
-        output.store_hash()
-        depsfile = utils.Depsfile(depfilename)
+    def file_arguments(self, output):
+        """
+        Return the list of the command line arguments that specify source,
+        output, and dependency files to be used for the subprocess call
+        """
+        return ["-d", self.depfilename(output),
+                "-o", output.filepath,
+                self.source_files[0].filepath]
+
+    def handle_dependencies(self, output):
+        depsfile = utils.Depsfile(self.depfilename(output))
         assert len(depsfile.rules) == 1, "Expecting only one rule in and openscad deps file"
-        assert len(depsfile.rules[0].outputs) == 1, "Expecting only one output to be specified in the openscad depsile"
+        assert len(depsfile.rules[0].outputs) == 1, "Expecting only one output to be specified in the openscad depsfile"
         assert depsfile.rules[0].outputs[0] == output, "depsfile output doens't match expected file"
         for dep in depsfile.rules[0].dependencies:
-            if dep not in export.source_files+export.dependencies:
-                export.add_dependency(dep, store_hash=True)
-        export.mark_dependencies_exhaustive()
-        self._all_output_files[output.filepath] = PROCESSED
-
-    def _process_freecad(self, export):
-        #TODO: Tidy up
-
-        outputs = export.output_files
-        sources = export.source_files
-        assert len(sources) == 1, "FreeCAD expects only one source file"
-        sourcefile = sources[0].filepath
-        assert len(export.app_options) == 0, "Cannot apply options to FreeCAD"
-        for parameter in export.parameters:
-            LOGGER.info("Cannot process parameters for FreeCAD skipping parameter %s",
+            if dep not in self.source_files+self.export.dependencies:
+                self.export.add_dependency(dep, store_hash=True)
+        self.export.mark_dependencies_exhaustive()
+
+    def print_output_on_success(self, ret):
+        """Overloaded as OpenSCAD writes everything to stderr"""
+        std_err = ret.stderr.decode('UTF-8')
+        print(std_err)
+
+
+class CadQueryExporter(BaseExporter):
+    """
+    This is a exporter class for CadQuery.
+    """
+
+    name = "CadQuery"
+    executable = "cq-cli"
+    min_outputs = 1
+    max_outputs = None
+    min_sources = 1
+    max_sources = 1
+
+    @property
+    def parameter_agruments(self):
+        """
+        Parse the parameters into a list of the command line arguments to be used
+        for the subprocess call
+        """
+        if len(self.export.parameters) == 0:
+            return []
+
+        # Process the parameters into a string that cq-cli will understand
+        params = ""
+        for param in self.export.parameters:
+            params += f"{param}:{self.export.parameters[param]};"
+        return ["--params", params]
+
+    def file_arguments(self, output):
+        """
+        Return the list of the command line arguments that specify source and
+        output files to be used for the subprocess call
+        """
+        source = self.source_files[0]
+        return [ "--infile", source.filepath, "--outfile", output.filepath]
+
+class FreeCADExporter(BaseExporter):
+    """
+    This is a exporter class for FreeCAD.
+    """
+
+    name = "FreeCAD"
+    executable = "freecadcmd"
+    min_outputs = 1
+    max_outputs = None
+    min_sources = 1
+    max_sources = 1
+
+    def __init__(self, export, headless=False):
+        super().__init__(export, headless)
+        self.selection = "Body"
+
+    @property
+    def parameter_agruments(self):
+        """
+        Parse the parameters into a list of the command line arguments to be used
+        for the subprocess call
+        """
+        for parameter in self.export.parameters:
+            if parameter == "object-selected":
+                self.selection = self.export.parameters[parameter]
+                continue
+            LOGGER.info("Cannot process parameter %s for FreeCAD, skipping",
                         parameter)
-            continue
+        return []
+
+    def file_arguments(self, output):
+        """
+        Return the list of the command line arguments that specify source and
+        output files to be used for the subprocess call. In this FreeCAD case
+        as we are using a macro we only spefify the macro that was created in
+        _create_macro. This macro sets the source and export files
+        """
+        macropath = self._create_macro(output)
+        return [macropath]
+
+    def _create_macro(self, output):
+        """Freecad doesn't provide a cli for exporting so a macro must be created"""
 
-        for outfile_obj in outputs:
-            outfile = outfile_obj.filepath
-            utils.add_directory_if_needed(outfile_obj.filepath)
-            if outfile.lower().endswith('.stp') or outfile.lower().endswith('.step'):
-                macro = (f"doc = FreeCAD.openDocument('{sourcefile}')\n"
-                         "body = doc.getObject('Body')\n"
-                         f"body.Shape.exportStep('{outfile}')\n")
-            elif outfile.lower().endswith('.stl'):
-                macro = ("from FreeCAD import Mesh\n"
-                         f"doc = FreeCAD.openDocument('{sourcefile}')\n"
-                         "body = doc.getObject('Body')\n"
-                         f"Mesh.export([body], '{outfile}')\n")
-            tmpdir = gettempdir()
-            macropath = path.join(tmpdir, "export.FCMacro")
-            with open(macropath, 'w', encoding="utf-8") as file_obj:
-                file_obj.write(macro)
-            subprocess.run(["freecadcmd", macropath], check=True)
-            outfile_obj.store_hash()
-            self._all_output_files[outfile] = PROCESSED
+        sourcefile = self.source_files[0].filepath
+        outfile  = output.filepath
+        selection_macro = (f"doc = FreeCAD.openDocument('{sourcefile}')\n"
+                           f"object = doc.getObjectsByLabel('{self.selection}')[0]\n")
+
+        if outfile.lower().endswith('.stp') or outfile.lower().endswith('.step'):
+            macro = (selection_macro +
+                     f"object.Shape.exportStep('{outfile}')\n")
+        elif outfile.lower().endswith('.stl'):
+            macro = ("from FreeCAD import Mesh\n" +
+                     selection_macro +
+                     f"Mesh.export([object], '{outfile}')\n")
+
+        tmpdir = gettempdir()
+        macropath = path.join(tmpdir, "export.FCMacro")
+        with open(macropath, 'w', encoding="utf-8") as file_obj:
+            file_obj.write(macro)
+        return macropath
+
+    def check_return_for_hidden_error(self, ret, output):
+        """freecadcmd outputs zero error code even if script failed."""
+        std_err = ret.stderr.decode('UTF-8')
+        if (len(std_err)) > 0:
+            raise RuntimeError(f"\n\n{self.name} failed create file: {output.filepath}"
+                               f" with error:\n\n{std_err}")
```

### Comparing `exsource_tools-0.0.5/exsource_tools/utils.py` & `exsource_tools-0.0.6/exsource_tools/utils.py`

 * *Files identical despite different names*

### Comparing `exsource_tools-0.0.5/exsource_tools.egg-info/PKG-INFO` & `exsource_tools-0.0.6/exsource_tools.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: exsource-tools
-Version: 0.0.5
+Version: 0.0.6
 Summary: Python tools for using Exsource files
 Home-page: https://gitlab.com/gitbuilding/exsource-tools
 Author: Julian Stirling
 Author-email: julian@julianstirling.co.uk
 License: LGPLv3
 Project-URL: Bug Tracker, https://gitlab.com/gitbuilding/exsource-tools/issues
 Project-URL: Source Code, https://gitlab.com/gitbuilding/exsource-tools
@@ -17,17 +17,50 @@
 License-File: LICENSE
 Requires-Dist: argparse
 Requires-Dist: pyyaml>=5.1
 Requires-Dist: jsonschema
 Provides-Extra: dev
 Requires-Dist: pylint; extra == "dev"
 Requires-Dist: twine; extra == "dev"
+Requires-Dist: colorama; extra == "dev"
 
 # ExSource-Tools
 
 An experimental Python library for validating and using the [ExSource Specification](https://gitlab.com/gitbuilding/exsourcespec) which is in the early stage of development.
 
+## Commands
+
+### Make
+
 This packages adds the following command:
 
-    exsource-make exsource.yml
+    exsource-make
+
+This will attempt to process `exsource-def.yml` to create inputs. The first instance of this proof of principle implementation supports OpenSCAD, FreeCAD, and CadQuery files. Each of these must be installed separately if they are to be used.
+
+***FreeCAD***  
+By default FreeCAD exporter will expect there to be a PartDesign Body called `Body`, it can export this to STEP and/or STL. The body to export can be changed by specifying the label of the object with `object-selected` as a parameter. For example:
+```yaml
+frame:
+    name: Main frame
+    description: >
+        This frame holds the shelf brackets and shelves.
+    output-files:
+        - output/frame.step
+        - output/frame.stl
+    source-files:
+        - assets/frame.FCStd
+    parameters:
+        object-selected: "Frame"
+    application: freecad
+```
+
+***CadQuery***  
+The CardQuery export is performed via [cq-cli](https://github.com/CadQuery/cq-cli)
+
+### Check
+
+You can also use the command:
+
+    exsource-check
 
-This will attempt to process `exsource.yml` to create inputs. The first instance of this proof of principle implementation supports OpenSCAD and some FreeCAD files. FreeCAD exporter will expect there to be a PartDesign Body called `Body`, it can export this to STEP and/or STL.
+This will specify what would happen if `exsource-make` was run.
```

### Comparing `exsource_tools-0.0.5/setup.py` & `exsource_tools-0.0.6/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''Setup for the module'''
 
 __author__ = 'Julian Stirling'
-__version__ = '0.0.5'
+__version__ = '0.0.6'
 
 import sys
 from os import path
 import glob
 from setuptools import setup, find_packages
 
 def install():
@@ -40,14 +40,14 @@
           url='https://gitlab.com/gitbuilding/exsource-tools',
           project_urls={"Bug Tracker": "https://gitlab.com/gitbuilding/exsource-tools/issues",
                         "Source Code": "https://gitlab.com/gitbuilding/exsource-tools"},
           classifiers=['Development Status :: 5 - Production/Stable',
                        'License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)',
                        'Programming Language :: Python :: 3.7'],
           install_requires=['argparse', 'pyyaml>=5.1', 'jsonschema'],
-          extras_require={'dev': ['pylint', 'twine']},
+          extras_require={'dev': ['pylint', 'twine', 'colorama']},
           python_requires=">=3.7",
           entry_points={'console_scripts': ['exsource-make = exsource_tools.cli:make',
                                             'exsource-check = exsource_tools.cli:check',]})
 
 if __name__ == "__main__":
     install()
```

