# Comparing `tmp/pypechain-0.0.8.tar.gz` & `tmp/pypechain-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypechain-0.0.8.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "pypechain-0.0.9.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pypechain-0.0.8.tar` & `pypechain-0.0.9.tar`

### file list

```diff
@@ -1,39 +1,50 @@
--rw-r--r--   0        0        0     1196 2023-11-13 16:03:17.618572 pypechain-0.0.8/README.md
--rw-r--r--   0        0        0      226 2023-10-11 21:21:15.016685 pypechain-0.0.8/pypechain/__init__.py
--rw-r--r--   0        0        0      800 2023-11-16 20:21:44.830846 pypechain-0.0.8/pypechain/foundry/types.py
--rw-r--r--   0        0        0      611 2023-11-16 20:21:44.831082 pypechain-0.0.8/pypechain/foundry/utilities.py
--rw-r--r--   0        0        0     3788 2023-11-16 22:39:31.968658 pypechain-0.0.8/pypechain/main.py
--rw-r--r--   0        0        0        0 2023-10-11 15:44:18.919551 pypechain-0.0.8/pypechain/render/__init__.py
--rw-r--r--   0        0        0     5470 2023-11-17 22:00:36.665861 pypechain-0.0.8/pypechain/render/contract.py
--rw-r--r--   0        0        0     4187 2023-11-16 20:21:44.832063 pypechain-0.0.8/pypechain/render/contract_test.py
--rw-r--r--   0        0        0     1305 2023-11-16 22:39:31.968809 pypechain-0.0.8/pypechain/render/main.py
--rw-r--r--   0        0        0     1430 2023-11-17 16:01:00.337491 pypechain-0.0.8/pypechain/render/types.py
--rw-r--r--   0        0        0      280 2023-11-16 20:21:44.832571 pypechain-0.0.8/pypechain/solc/types.py
--rw-r--r--   0        0        0      841 2023-11-16 20:21:44.832875 pypechain-0.0.8/pypechain/solc/utilities.py
--rw-r--r--   0        0        0      178 2023-11-16 20:21:44.833233 pypechain-0.0.8/pypechain/templates/contract.py/abi.py.jinja2
--rw-r--r--   0        0        0     1169 2023-11-17 16:56:16.916945 pypechain-0.0.8/pypechain/templates/contract.py/base.py.jinja2
--rw-r--r--   0        0        0      656 2023-11-16 20:21:44.834297 pypechain-0.0.8/pypechain/templates/contract.py/contract.py.jinja2
--rw-r--r--   0        0        0     2270 2023-11-17 22:00:36.666141 pypechain-0.0.8/pypechain/templates/contract.py/functions.py.jinja2
--rw-r--r--   0        0        0     1466 2023-11-10 18:36:25.870575 pypechain-0.0.8/pypechain/templates/types.py.jinja2
--rw-r--r--   0        0        0        0 2023-11-16 20:21:44.834672 pypechain-0.0.8/pypechain/test/__init__.py
--rw-r--r--   0        0        0     4212 2023-11-10 21:42:49.583018 pypechain-0.0.8/pypechain/test/overloading/.build/__local__.json
--rw-r--r--   0        0        0      188 2023-11-16 20:21:44.835128 pypechain-0.0.8/pypechain/test/overloading/README.md
--rw-r--r--   0        0        0        0 2023-11-16 20:21:44.835171 pypechain-0.0.8/pypechain/test/overloading/__init__.py
--rw-r--r--   0        0        0     4904 2023-11-16 20:21:44.835467 pypechain-0.0.8/pypechain/test/overloading/abis/OverloadedMethods.json
--rw-r--r--   0        0        0      598 2023-11-16 20:21:44.835775 pypechain-0.0.8/pypechain/test/overloading/contracts/OverloadedMethods.sol
--rw-r--r--   0        0        0     1940 2023-11-16 20:21:44.835947 pypechain-0.0.8/pypechain/test/overloading/test_overloading.py
--rw-r--r--   0        0        0     6153 2023-11-16 20:21:44.836224 pypechain-0.0.8/pypechain/test/overloading/types/OverloadedMethodsContract.py
--rw-r--r--   0        0        0      682 2023-11-16 20:21:44.836410 pypechain-0.0.8/pypechain/test/overloading/types/OverloadedMethodsTypes.py
--rw-r--r--   0        0        0        0 2023-11-16 20:21:44.836440 pypechain-0.0.8/pypechain/test/overloading/types/__init__.py
--rw-r--r--   0        0        0     2861 2023-11-16 20:21:44.836720 pypechain-0.0.8/pypechain/test/test_file_recursion.py
--rw-r--r--   0        0        0        0 2023-11-08 16:49:42.136820 pypechain-0.0.8/pypechain/utilities/__init__.py
--rw-r--r--   0        0        0    20455 2023-11-17 22:00:36.666462 pypechain-0.0.8/pypechain/utilities/abi.py
--rw-r--r--   0        0        0     1119 2023-11-10 18:36:25.870962 pypechain-0.0.8/pypechain/utilities/abi_test.py
--rw-r--r--   0        0        0      451 2023-11-10 15:18:08.100025 pypechain-0.0.8/pypechain/utilities/file.py
--rw-r--r--   0        0        0     2438 2023-11-17 16:56:16.917520 pypechain-0.0.8/pypechain/utilities/format.py
--rw-r--r--   0        0        0      757 2023-11-16 20:21:44.837355 pypechain-0.0.8/pypechain/utilities/json.py
--rw-r--r--   0        0        0      949 2023-10-11 15:44:18.920848 pypechain-0.0.8/pypechain/utilities/sort.py
--rw-r--r--   0        0        0      423 2023-11-10 18:36:25.871266 pypechain-0.0.8/pypechain/utilities/templates.py
--rw-r--r--   0        0        0     3831 2023-11-17 16:56:16.917673 pypechain-0.0.8/pypechain/utilities/types.py
--rw-r--r--   0        0        0     1466 2023-11-17 22:01:54.986538 pypechain-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     2605 1970-01-01 00:00:00.000000 pypechain-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1196 2023-11-13 16:03:17.618572 pypechain-0.0.9/README.md
+-rw-r--r--   0        0        0      226 2023-10-11 21:21:15.016685 pypechain-0.0.9/pypechain/__init__.py
+-rw-r--r--   0        0        0      800 2023-11-16 20:21:44.830846 pypechain-0.0.9/pypechain/foundry/types.py
+-rw-r--r--   0        0        0      611 2023-11-16 20:21:44.831082 pypechain-0.0.9/pypechain/foundry/utilities.py
+-rw-r--r--   0        0        0     4433 2023-11-20 23:11:23.201803 pypechain-0.0.9/pypechain/main.py
+-rw-r--r--   0        0        0        0 2023-10-11 15:44:18.919551 pypechain-0.0.9/pypechain/render/__init__.py
+-rw-r--r--   0        0        0     5511 2023-11-22 00:00:00.384507 pypechain-0.0.9/pypechain/render/contract.py
+-rw-r--r--   0        0        0     4187 2023-11-16 20:21:44.832063 pypechain-0.0.9/pypechain/render/contract_test.py
+-rw-r--r--   0        0        0     1623 2023-11-20 23:11:23.201996 pypechain-0.0.9/pypechain/render/main.py
+-rw-r--r--   0        0        0     1569 2023-11-20 23:11:23.202166 pypechain-0.0.9/pypechain/render/types.py
+-rw-r--r--   0        0        0      280 2023-11-16 20:21:44.832571 pypechain-0.0.9/pypechain/solc/types.py
+-rw-r--r--   0        0        0      841 2023-11-16 20:21:44.832875 pypechain-0.0.9/pypechain/solc/utilities.py
+-rw-r--r--   0        0        0      178 2023-11-16 20:21:44.833233 pypechain-0.0.9/pypechain/templates/contract.py/abi.py.jinja2
+-rw-r--r--   0        0        0     2952 2023-11-22 00:00:00.384897 pypechain-0.0.9/pypechain/templates/contract.py/base.py.jinja2
+-rw-r--r--   0        0        0     1071 2023-11-22 00:00:00.385103 pypechain-0.0.9/pypechain/templates/contract.py/contract.py.jinja2
+-rw-r--r--   0        0        0     4407 2023-11-22 00:00:00.385295 pypechain-0.0.9/pypechain/templates/contract.py/functions.py.jinja2
+-rw-r--r--   0        0        0      112 2023-11-20 23:11:23.202387 pypechain-0.0.9/pypechain/templates/init.py.jinja2
+-rw-r--r--   0        0        0     1466 2023-11-10 18:36:25.870575 pypechain-0.0.9/pypechain/templates/types.py.jinja2
+-rw-r--r--   0        0        0        0 2023-11-16 20:21:44.834672 pypechain-0.0.9/pypechain/test/__init__.py
+-rw-r--r--   0        0        0     4212 2023-11-10 21:42:49.583018 pypechain-0.0.9/pypechain/test/overloading/.build/__local__.json
+-rw-r--r--   0        0        0      188 2023-11-16 20:21:44.835128 pypechain-0.0.9/pypechain/test/overloading/README.md
+-rw-r--r--   0        0        0        0 2023-11-16 20:21:44.835171 pypechain-0.0.9/pypechain/test/overloading/__init__.py
+-rw-r--r--   0        0        0     4904 2023-11-16 20:21:44.835467 pypechain-0.0.9/pypechain/test/overloading/abis/OverloadedMethods.json
+-rw-r--r--   0        0        0      598 2023-11-16 20:21:44.835775 pypechain-0.0.9/pypechain/test/overloading/contracts/OverloadedMethods.sol
+-rw-r--r--   0        0        0     1940 2023-11-20 18:37:49.567772 pypechain-0.0.9/pypechain/test/overloading/test_overloading.py
+-rw-r--r--   0        0        0     6153 2023-11-16 20:21:44.836224 pypechain-0.0.9/pypechain/test/overloading/types/OverloadedMethodsContract.py
+-rw-r--r--   0        0        0      682 2023-11-16 20:21:44.836410 pypechain-0.0.9/pypechain/test/overloading/types/OverloadedMethodsTypes.py
+-rw-r--r--   0        0        0        0 2023-11-16 20:21:44.836440 pypechain-0.0.9/pypechain/test/overloading/types/__init__.py
+-rw-r--r--   0        0        0     4212 2023-11-21 16:13:51.810652 pypechain-0.0.9/pypechain/test/return_types/.build/__local__.json
+-rw-r--r--   0        0        0      170 2023-11-22 00:00:00.385572 pypechain-0.0.9/pypechain/test/return_types/README.md
+-rw-r--r--   0        0        0        0 2023-11-22 00:00:00.385626 pypechain-0.0.9/pypechain/test/return_types/__init__.py
+-rw-r--r--   0        0        0    23437 2023-11-22 00:00:00.386043 pypechain-0.0.9/pypechain/test/return_types/abis/ReturnTypes.json
+-rw-r--r--   0        0        0     3236 2023-11-22 00:00:00.386292 pypechain-0.0.9/pypechain/test/return_types/contracts/ReturnTypes.sol
+-rw-r--r--   0        0        0     4064 2023-11-22 00:00:00.386432 pypechain-0.0.9/pypechain/test/return_types/test_returntypes.py
+-rw-r--r--   0        0        0    47144 2023-11-22 00:00:00.386673 pypechain-0.0.9/pypechain/test/return_types/types/ReturnTypesContract.py
+-rw-r--r--   0        0        0     1016 2023-11-22 00:00:00.386821 pypechain-0.0.9/pypechain/test/return_types/types/ReturnTypesTypes.py
+-rw-r--r--   0        0        0      113 2023-11-22 00:00:00.386959 pypechain-0.0.9/pypechain/test/return_types/types/__init__.py
+-rw-r--r--   0        0        0     2861 2023-11-16 20:21:44.836720 pypechain-0.0.9/pypechain/test/test_file_recursion.py
+-rw-r--r--   0        0        0        0 2023-11-08 16:49:42.136820 pypechain-0.0.9/pypechain/utilities/__init__.py
+-rw-r--r--   0        0        0    20455 2023-11-17 22:00:36.666462 pypechain-0.0.9/pypechain/utilities/abi.py
+-rw-r--r--   0        0        0     1119 2023-11-10 18:36:25.870962 pypechain-0.0.9/pypechain/utilities/abi_test.py
+-rw-r--r--   0        0        0     1634 2023-11-22 00:00:00.387193 pypechain-0.0.9/pypechain/utilities/conversion.py
+-rw-r--r--   0        0        0      451 2023-11-10 15:18:08.100025 pypechain-0.0.9/pypechain/utilities/file.py
+-rw-r--r--   0        0        0     2525 2023-11-22 00:00:00.387416 pypechain-0.0.9/pypechain/utilities/format.py
+-rw-r--r--   0        0        0      757 2023-11-16 20:21:44.837355 pypechain-0.0.9/pypechain/utilities/json.py
+-rw-r--r--   0        0        0      949 2023-10-11 15:44:18.920848 pypechain-0.0.9/pypechain/utilities/sort.py
+-rw-r--r--   0        0        0      423 2023-11-10 18:36:25.871266 pypechain-0.0.9/pypechain/utilities/templates.py
+-rw-r--r--   0        0        0     3843 2023-11-22 00:00:00.387609 pypechain-0.0.9/pypechain/utilities/types.py
+-rw-r--r--   0        0        0     1466 2023-11-22 00:00:19.477264 pypechain-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     2605 1970-01-01 00:00:00.000000 pypechain-0.0.9/PKG-INFO
```

### Comparing `pypechain-0.0.8/README.md` & `pypechain-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `pypechain-0.0.8/pypechain/foundry/types.py` & `pypechain-0.0.9/pypechain/foundry/types.py`

 * *Files identical despite different names*

### Comparing `pypechain-0.0.8/pypechain/foundry/utilities.py` & `pypechain-0.0.9/pypechain/foundry/utilities.py`

 * *Files identical despite different names*

### Comparing `pypechain-0.0.8/pypechain/main.py` & `pypechain-0.0.9/pypechain/main.py`

 * *Files 21% similar despite different names*

```diff
@@ -7,14 +7,17 @@
 import sys
 from pathlib import Path
 from typing import NamedTuple, Sequence
 
 from web3.exceptions import NoABIFunctionsFound
 
 from pypechain.render.main import render_files
+from pypechain.utilities.file import write_string_to_file
+from pypechain.utilities.format import apply_black_formatting
+from pypechain.utilities.templates import get_jinja_env
 
 
 def main(argv: Sequence[str] | None = None) -> None:
     """Generates class files for a given abi.
 
     Arguments
     ---------
@@ -28,34 +31,49 @@
 
     abi_file_path, output_dir, line_length = parse_arguments(argv)
 
     # Create/clear the output directory
     setup_directory(output_dir)
 
     # List to store all JSON ABI files to be processed
-    json_files_to_process = []
+    json_files_to_process: list[Path] = []
 
     # Check if provided path is a directory or file
     if os.path.isdir(abi_file_path):
         # If directory, gather all JSON files recursively in the directory
         json_files_to_process.extend(gather_json_files(abi_file_path))
     else:
         # Otherwise, add the single file to the list
         json_files_to_process.append(Path(abi_file_path))
 
+    file_names: list[str] = []
+
     # Now process all gathered files
     for json_file in json_files_to_process:
         try:
-            render_files(str(json_file), output_dir, line_length)
+            rendered_file_names = render_files(str(json_file), output_dir, line_length)
+            file_names.extend(rendered_file_names)
         except NoABIFunctionsFound:
             print(f"No ABI Functions found in {json_file}, skipping...")
         except BaseException as err:
             print(f"Error creating types for {json_file}")
             raise err
 
+    # Finally, render the __init__.py file
+    render_init_file(output_dir, file_names, line_length)
+
+
+def render_init_file(output_dir: str, file_names: list[str], line_length):
+    """Creates an __init__.py file that imports all other files."""
+    env = get_jinja_env()
+    init_template = env.get_template("init.py.jinja2")
+    init_code = init_template.render(file_names=file_names)
+    formatted_init_code = apply_black_formatting(init_code, line_length)
+    write_string_to_file(f"{output_dir}/__init__.py", formatted_init_code)
+
 
 def gather_json_files(directory: str) -> list:
     """Gathers all JSON files in the specified directory and its subdirectories."""
     return list(Path(directory).rglob("*.json"))
 
 
 def setup_directory(directory: str) -> None:
@@ -64,19 +82,14 @@
     # If the directory exists, remove it
     if os.path.exists(directory):
         shutil.rmtree(directory)
 
     # Create the directory
     os.makedirs(directory)
 
-    # Create an empty __init__.py file in the directory
-    init_file_path = os.path.join(directory, "__init__.py")
-    with open(init_file_path, "a", encoding="utf-8"):
-        pass
-
 
 class Args(NamedTuple):
     """Command line arguments for pypechain."""
 
     abi_file_path: str
     output_dir: str
     line_length: int
```

### Comparing `pypechain-0.0.8/pypechain/render/contract.py` & `pypechain-0.0.9/pypechain/render/contract.py`

 * *Files 3% similar despite different names*

```diff
@@ -71,14 +71,15 @@
         functions=function_datas,
     )
 
     # Render the template
     return templates.base_template.render(
         contract_name=contract_name,
         structs_used=structs_used,
+        structs_for_abi=structs_for_abi,
         has_overloading=has_overloading,
         has_bytecode=has_bytecode,
         functions_block=functions_block,
         abi_block=abi_block,
         contract_block=contract_block,
         # TODO: use this data to add a typed constructor
         # constructor_data=constructor_data,
```

### Comparing `pypechain-0.0.8/pypechain/render/contract_test.py` & `pypechain-0.0.9/pypechain/render/contract_test.py`

 * *Files identical despite different names*

### Comparing `pypechain-0.0.8/pypechain/render/main.py` & `pypechain-0.0.9/pypechain/render/main.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,33 +1,39 @@
 """Functions to render Python files from an abi usng a jinja2 template."""
 
 import os
 from pathlib import Path
 
-
 from pypechain.render.contract import render_contract_file
 from pypechain.render.types import render_types_file
 from pypechain.utilities.file import write_string_to_file
 from pypechain.utilities.format import apply_black_formatting
 
 
-def render_files(abi_file_path: str, output_dir: str, line_length: int) -> None:
+def render_files(abi_file_path: str, output_dir: str, line_length: int) -> list[str]:
     """Processes a single JSON file to generate class and types files."""
 
     # get names
     file_path = Path(abi_file_path)
     output_path = Path(output_dir)
     filename = file_path.name
     contract_name = os.path.splitext(filename)[0]
     contract_path = output_path.joinpath(f"{contract_name}")
 
     # render the code
     rendered_contract_code = render_contract_file(contract_name, file_path)
+    # TODO: if there are no types generated, then this should return None
     rendered_types_code = render_types_file(contract_name, file_path)
 
-    # Format the generated code using Black
+    file_names: list[str] = []
+    # Format the generated code using Black and rite the code to file
     formatted_contract_code = apply_black_formatting(rendered_contract_code, line_length)
-    formatted_types_code = apply_black_formatting(rendered_types_code, line_length)
-
-    # Write the code to file
     write_string_to_file(f"{contract_path}Contract.py", formatted_contract_code)
-    write_string_to_file(f"{contract_path}Types.py", formatted_types_code)
+    file_names.append(f"{contract_name}Contract")
+
+    # TODO: write tests for this conditional write.
+    if rendered_types_code:
+        formatted_types_code = apply_black_formatting(rendered_types_code, line_length)
+        write_string_to_file(f"{contract_path}Types.py", formatted_types_code)
+        file_names.append(f"{contract_name}Types")
+
+    return file_names
```

### Comparing `pypechain-0.0.8/pypechain/render/types.py` & `pypechain-0.0.9/pypechain/render/types.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 """Functions to render Python types from an abi usng a jinja2 template."""
+from __future__ import annotations
+
 from dataclasses import asdict
 from pathlib import Path
 
 from pypechain.utilities.abi import get_events_for_abi, get_structs_for_abi, load_abi_from_file
 from pypechain.utilities.templates import get_jinja_env
 
 
-def render_types_file(contract_name: str, abi_file_path: Path) -> str:
+def render_types_file(contract_name: str, abi_file_path: Path) -> str | None:
     """Returns the serialized code of the types file to be generated.
 
     Arguments
     ---------
     contract_name : str
         The name of the contract to be parsed.
     types_template : Template
@@ -29,16 +31,20 @@
     abi, _ = load_abi_from_file(abi_file_path)
 
     structs_by_name = get_structs_for_abi(abi)
     structs_list = list(structs_by_name.values())
     structs = [asdict(struct) for struct in structs_list]
     events = [asdict(event) for event in get_events_for_abi(abi)]
     has_events = bool(events)
+    has_structs = bool(structs)
     has_event_params = any(len(event["inputs"]) > 0 for event in events)
 
+    if not has_events and not has_structs:
+        return None
+
     return types_template.render(
         contract_name=contract_name,
         structs=structs,
         events=events,
         has_events=has_events,
         has_event_params=has_event_params,
     )
```

### Comparing `pypechain-0.0.8/pypechain/solc/utilities.py` & `pypechain-0.0.9/pypechain/solc/utilities.py`

 * *Files identical despite different names*

### Comparing `pypechain-0.0.8/pypechain/templates/contract.py/contract.py.jinja2` & `pypechain-0.0.9/pypechain/templates/contract.py/contract.py.jinja2`

 * *Files 22% similar despite different names*

```diff
@@ -6,15 +6,23 @@
     bytecode: bytes = HexBytes({{contract_name | lower}}_bytecode)
     {%- endif %}
 
     def __init__(self, address: ChecksumAddress | None = None) -> None:
         try:
             # Initialize parent Contract class
             super().__init__(address=address)
+            self.functions = {{contract_name}}ContractFunctions({{contract_name | lower}}_abi, self.w3, address)
 
         except FallbackNotFound:
             print("Fallback function not found. Continuing...")
 
     # TODO: add events
     # events: ERC20ContractEvents
 
-    functions: {{contract_name}}ContractFunctions
+    functions: {{contract_name}}ContractFunctions
+
+    @classmethod
+    def factory(cls, w3: Web3, class_name: str | None = None, **kwargs: Any) -> Type[Self]:
+        contract = super().factory(w3, class_name, **kwargs)
+        contract.functions = {{contract_name}}ContractFunctions({{contract_name | lower}}_abi, w3, None)
+
+        return contract
```

### Comparing `pypechain-0.0.8/pypechain/templates/types.py.jinja2` & `pypechain-0.0.9/pypechain/templates/types.py.jinja2`

 * *Files identical despite different names*

### Comparing `pypechain-0.0.8/pypechain/test/overloading/.build/__local__.json` & `pypechain-0.0.9/pypechain/test/overloading/.build/__local__.json`

 * *Files identical despite different names*

### Comparing `pypechain-0.0.8/pypechain/test/overloading/abis/OverloadedMethods.json` & `pypechain-0.0.9/pypechain/test/overloading/abis/OverloadedMethods.json`

 * *Files identical despite different names*

### Comparing `pypechain-0.0.8/pypechain/test/overloading/contracts/OverloadedMethods.sol` & `pypechain-0.0.9/pypechain/test/overloading/contracts/OverloadedMethods.sol`

 * *Files identical despite different names*

### Comparing `pypechain-0.0.8/pypechain/test/overloading/test_overloading.py` & `pypechain-0.0.9/pypechain/test/overloading/test_overloading.py`

 * *Files identical despite different names*

### Comparing `pypechain-0.0.8/pypechain/test/overloading/types/OverloadedMethodsContract.py` & `pypechain-0.0.9/pypechain/test/overloading/types/OverloadedMethodsContract.py`

 * *Files identical despite different names*

### Comparing `pypechain-0.0.8/pypechain/test/overloading/types/OverloadedMethodsTypes.py` & `pypechain-0.0.9/pypechain/test/overloading/types/OverloadedMethodsTypes.py`

 * *Files identical despite different names*

### Comparing `pypechain-0.0.8/pypechain/test/test_file_recursion.py` & `pypechain-0.0.9/pypechain/test/test_file_recursion.py`

 * *Files identical despite different names*

### Comparing `pypechain-0.0.8/pypechain/utilities/abi.py` & `pypechain-0.0.9/pypechain/utilities/abi.py`

 * *Files identical despite different names*

### Comparing `pypechain-0.0.8/pypechain/utilities/abi_test.py` & `pypechain-0.0.9/pypechain/utilities/abi_test.py`

 * *Files identical despite different names*

### Comparing `pypechain-0.0.8/pypechain/utilities/format.py` & `pypechain-0.0.9/pypechain/utilities/format.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Formatting utilities."""
 import keyword
 
 import black
+from black.report import NothingChanged
 
 
 def avoid_python_keywords(name: str) -> str:
     """Make sure the variable name is not a reserved Python word.  If it is, prepend with an
     underscore.
 
     Arguments
@@ -124,7 +125,9 @@
     """
     try:
         return black.format_file_contents(code, fast=False, mode=black.Mode(line_length=line_length))
     except ValueError as exc:
         print(f"cannot format with Black\n code:\n{code}")
         print(f"{exc=}")
         return code
+    except NothingChanged:
+        return code
```

### Comparing `pypechain-0.0.8/pypechain/utilities/json.py` & `pypechain-0.0.9/pypechain/utilities/json.py`

 * *Files identical despite different names*

### Comparing `pypechain-0.0.8/pypechain/utilities/sort.py` & `pypechain-0.0.9/pypechain/utilities/sort.py`

 * *Files identical despite different names*

### Comparing `pypechain-0.0.8/pypechain/utilities/types.py` & `pypechain-0.0.9/pypechain/utilities/types.py`

 * *Files 1% similar despite different names*

```diff
@@ -122,13 +122,14 @@
 
     for function_data in function_datas:
         for signature_data in function_data["signature_datas"]:
             # Check input types
             for input_type in signature_data["input_types"]:
                 if input_type in known_types:
                     matching_types.append(input_type)
+
             # Check output types
             for output_type in signature_data["output_types"]:
                 if output_type in known_types:
                     matching_types.append(output_type)
 
-    return matching_types
+    return list(set(matching_types))
```

### Comparing `pypechain-0.0.8/pyproject.toml` & `pypechain-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 
 name = "pypechain"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
     { name = "Matthew Brown", email = "matt@delv.tech" },
     { name = "Dylan Paiton", email = "dylan@delv.tech" },
     { name = "Sheng Lundquist", email = "sheng@delv.tech" },
     { name = "Mihai Cosma", email = "mihai@delv.tech" },
 ]
 description = "Codegen python interfaces for web3.py contracts."
```

### Comparing `pypechain-0.0.8/PKG-INFO` & `pypechain-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypechain
-Version: 0.0.8
+Version: 0.0.9
 Summary: Codegen python interfaces for web3.py contracts.
 Author-email: Matthew Brown <matt@delv.tech>, Dylan Paiton <dylan@delv.tech>, Sheng Lundquist <sheng@delv.tech>, Mihai Cosma <mihai@delv.tech>
 Requires-Python: >=3.10, <3.11
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pypechain Version: 0.0.8 Summary: Codegen python
+Metadata-Version: 2.1 Name: pypechain Version: 0.0.9 Summary: Codegen python
 interfaces for web3.py contracts. Author-email: Matthew Brown
 delv.tech>, Dylan Paiton
 delv.tech>, Sheng Lundquist
 delv.tech>, Mihai Cosma
 delv.tech> Requires-Python: >=3.10, <3.11 Description-Content-Type: text/
 markdown Classifier: Programming Language :: Python :: 3 Classifier: License ::
 OSI Approved :: Apache Software License Classifier: Operating System :: OS
```

