# Comparing `tmp/funky_modifiers-0.1.7.tar.gz` & `tmp/funky_modifiers-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "funky_modifiers-0.1.7.tar", last modified: Sun May  5 21:37:34 2024, max compression
+gzip compressed data, was "funky_modifiers-0.1.8.tar", last modified: Thu May  9 11:17:07 2024, max compression
```

## Comparing `funky_modifiers-0.1.7.tar` & `funky_modifiers-0.1.8.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxrwxrwx   0        0        0        0 2024-05-05 21:37:33.999837 funky_modifiers-0.1.7/
--rw-rw-rw-   0        0        0     1525 2024-02-25 05:24:52.000000 funky_modifiers-0.1.7/LICENSE
--rw-rw-rw-   0        0        0       37 2024-05-05 20:43:12.000000 funky_modifiers-0.1.7/MANIFEST.in
--rw-rw-rw-   0        0        0      474 2024-05-05 21:37:33.998845 funky_modifiers-0.1.7/PKG-INFO
--rw-rw-rw-   0        0        0      131 2024-05-05 19:24:08.000000 funky_modifiers-0.1.7/README.md
--rw-rw-rw-   0        0        0       13 2024-05-05 21:32:06.000000 funky_modifiers-0.1.7/requirements.txt
--rw-rw-rw-   0        0        0       42 2024-05-05 21:37:33.999837 funky_modifiers-0.1.7/setup.cfg
--rw-rw-rw-   0        0        0      711 2024-05-05 21:37:27.000000 funky_modifiers-0.1.7/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-05 21:37:33.967595 funky_modifiers-0.1.7/src/
-drwxrwxrwx   0        0        0        0 2024-05-05 21:37:33.972060 funky_modifiers-0.1.7/src/funk_py/
--rw-rw-rw-   0        0        0       50 2023-12-27 12:08:10.000000 funky_modifiers-0.1.7/src/funk_py/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-05 21:37:33.975528 funky_modifiers-0.1.7/src/funk_py/modularity/
--rw-rw-rw-   0        0        0        0 2023-12-26 12:23:31.000000 funky_modifiers-0.1.7/src/funk_py/modularity/__init__.py
--rw-rw-rw-   0        0        0    39190 2024-05-05 15:25:24.000000 funky_modifiers-0.1.7/src/funk_py/modularity/basic_structures.py
--rw-rw-rw-   0        0        0     4500 2024-05-03 11:21:07.000000 funky_modifiers-0.1.7/src/funk_py/modularity/bespoke_properties.py
-drwxrwxrwx   0        0        0        0 2024-05-05 21:37:33.978009 funky_modifiers-0.1.7/src/funk_py/modularity/decoration/
--rw-rw-rw-   0        0        0      496 2024-02-24 19:47:42.000000 funky_modifiers-0.1.7/src/funk_py/modularity/decoration/__init__.py
--rw-rw-rw-   0        0        0     1260 2024-04-24 10:42:19.000000 funky_modifiers-0.1.7/src/funk_py/modularity/decoration/enum_modifiers.py
--rw-rw-rw-   0        0        0     9073 2024-02-25 05:13:05.000000 funky_modifiers-0.1.7/src/funk_py/modularity/decoration/init_modifiers.py
--rw-rw-rw-   0        0        0     2749 2023-12-26 12:23:31.000000 funky_modifiers-0.1.7/src/funk_py/modularity/decoration/transforming_list.py
--rw-rw-rw-   0        0        0     6475 2024-02-25 05:13:05.000000 funky_modifiers-0.1.7/src/funk_py/modularity/logging.py
--rw-rw-rw-   0        0        0    34949 2024-05-02 10:31:37.000000 funky_modifiers-0.1.7/src/funk_py/modularity/type_matching.py
-drwxrwxrwx   0        0        0        0 2024-05-05 21:37:33.980494 funky_modifiers-0.1.7/src/funk_py/sorting/
--rw-rw-rw-   0        0        0        0 2024-04-07 16:23:56.000000 funky_modifiers-0.1.7/src/funk_py/sorting/__init__.py
--rw-rw-rw-   0        0        0    20021 2024-05-05 16:10:17.000000 funky_modifiers-0.1.7/src/funk_py/sorting/converters.py
--rw-rw-rw-   0        0        0    18997 2024-05-05 11:30:10.000000 funky_modifiers-0.1.7/src/funk_py/sorting/dict_manip.py
--rw-rw-rw-   0        0        0    14818 2024-05-04 18:39:41.000000 funky_modifiers-0.1.7/src/funk_py/sorting/pieces.py
-drwxrwxrwx   0        0        0        0 2024-05-05 21:37:33.982967 funky_modifiers-0.1.7/src/funk_py/super_dicts/
--rw-rw-rw-   0        0        0     2139 2024-05-05 18:39:34.000000 funky_modifiers-0.1.7/src/funk_py/super_dicts/__init__.py
--rw-rw-rw-   0        0        0     8330 2024-03-03 18:51:02.000000 funky_modifiers-0.1.7/src/funk_py/super_dicts/drop_none_dict.py
--rw-rw-rw-   0        0        0     8942 2024-03-03 17:19:44.000000 funky_modifiers-0.1.7/src/funk_py/super_dicts/list_dict.py
--rw-rw-rw-   0        0        0     3583 2023-12-30 12:27:19.000000 funky_modifiers-0.1.7/src/funk_py/super_dicts/windowed_list.py
-drwxrwxrwx   0        0        0        0 2024-05-05 21:37:33.998343 funky_modifiers-0.1.7/src/funky_modifiers.egg-info/
--rw-rw-rw-   0        0        0      474 2024-05-05 21:37:33.000000 funky_modifiers-0.1.7/src/funky_modifiers.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1259 2024-05-05 21:37:33.000000 funky_modifiers-0.1.7/src/funky_modifiers.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-05 21:37:33.000000 funky_modifiers-0.1.7/src/funky_modifiers.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2024-05-05 21:37:33.000000 funky_modifiers-0.1.7/src/funky_modifiers.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-05 21:37:33.000000 funky_modifiers-0.1.7/src/funky_modifiers.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-05 21:37:33.997853 funky_modifiers-0.1.7/test/
--rw-rw-rw-   0        0        0    21040 2024-05-03 11:33:03.000000 funky_modifiers-0.1.7/test/test_check_dict_equality.py
--rw-rw-rw-   0        0        0    27490 2024-05-03 11:33:03.000000 funky_modifiers-0.1.7/test/test_check_list_equality.py
--rw-rw-rw-   0        0        0    21911 2024-04-27 15:34:29.000000 funky_modifiers-0.1.7/test/test_convert_tuplish_dict.py
--rw-rw-rw-   0        0        0    15212 2024-05-05 16:22:23.000000 funky_modifiers-0.1.7/test/test_converters.py
--rw-rw-rw-   0        0        0     3127 2024-04-24 10:25:16.000000 funky_modifiers-0.1.7/test/test_converts_enums.py
--rw-rw-rw-   0        0        0    12426 2024-03-03 19:25:27.000000 funky_modifiers-0.1.7/test/test_drop_none_dict.py
--rw-rw-rw-   0        0        0    26544 2024-03-03 19:25:27.000000 funky_modifiers-0.1.7/test/test_function_hash_and_equality.py
--rw-rw-rw-   0        0        0    12013 2024-04-12 20:31:58.000000 funky_modifiers-0.1.7/test/test_logs_vars.py
--rw-rw-rw-   0        0        0    35329 2024-05-02 11:24:45.000000 funky_modifiers-0.1.7/test/test_obj.py
--rw-rw-rw-   0        0        0    68867 2024-05-05 18:36:38.000000 funky_modifiers-0.1.7/test/test_pick.py
+drwxrwxrwx   0        0        0        0 2024-05-09 11:17:07.566620 funky_modifiers-0.1.8/
+-rw-rw-rw-   0        0        0     1525 2024-02-25 05:24:52.000000 funky_modifiers-0.1.8/LICENSE
+-rw-rw-rw-   0        0        0       37 2024-05-05 20:43:12.000000 funky_modifiers-0.1.8/MANIFEST.in
+-rw-rw-rw-   0        0        0      474 2024-05-09 11:17:07.565629 funky_modifiers-0.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0      131 2024-05-05 19:24:08.000000 funky_modifiers-0.1.8/README.md
+-rw-rw-rw-   0        0        0       13 2024-05-05 21:32:06.000000 funky_modifiers-0.1.8/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-05-09 11:17:07.567116 funky_modifiers-0.1.8/setup.cfg
+-rw-rw-rw-   0        0        0      711 2024-05-09 11:16:47.000000 funky_modifiers-0.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-09 11:17:07.510572 funky_modifiers-0.1.8/src/
+drwxrwxrwx   0        0        0        0 2024-05-09 11:17:07.522981 funky_modifiers-0.1.8/src/funk_py/
+-rw-rw-rw-   0        0        0       50 2023-12-27 12:08:10.000000 funky_modifiers-0.1.8/src/funk_py/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-09 11:17:07.530416 funky_modifiers-0.1.8/src/funk_py/modularity/
+-rw-rw-rw-   0        0        0        0 2023-12-26 12:23:31.000000 funky_modifiers-0.1.8/src/funk_py/modularity/__init__.py
+-rw-rw-rw-   0        0        0    39190 2024-05-05 15:25:24.000000 funky_modifiers-0.1.8/src/funk_py/modularity/basic_structures.py
+-rw-rw-rw-   0        0        0     4500 2024-05-03 11:21:07.000000 funky_modifiers-0.1.8/src/funk_py/modularity/bespoke_properties.py
+drwxrwxrwx   0        0        0        0 2024-05-09 11:17:07.534881 funky_modifiers-0.1.8/src/funk_py/modularity/decoration/
+-rw-rw-rw-   0        0        0      496 2024-02-24 19:47:42.000000 funky_modifiers-0.1.8/src/funk_py/modularity/decoration/__init__.py
+-rw-rw-rw-   0        0        0     1260 2024-04-24 10:42:19.000000 funky_modifiers-0.1.8/src/funk_py/modularity/decoration/enum_modifiers.py
+-rw-rw-rw-   0        0        0     9073 2024-02-25 05:13:05.000000 funky_modifiers-0.1.8/src/funk_py/modularity/decoration/init_modifiers.py
+-rw-rw-rw-   0        0        0     2749 2023-12-26 12:23:31.000000 funky_modifiers-0.1.8/src/funk_py/modularity/decoration/transforming_list.py
+-rw-rw-rw-   0        0        0     6475 2024-02-25 05:13:05.000000 funky_modifiers-0.1.8/src/funk_py/modularity/logging.py
+-rw-rw-rw-   0        0        0    34949 2024-05-02 10:31:37.000000 funky_modifiers-0.1.8/src/funk_py/modularity/type_matching.py
+drwxrwxrwx   0        0        0        0 2024-05-09 11:17:07.537857 funky_modifiers-0.1.8/src/funk_py/sorting/
+-rw-rw-rw-   0        0        0        0 2024-04-07 16:23:56.000000 funky_modifiers-0.1.8/src/funk_py/sorting/__init__.py
+-rw-rw-rw-   0        0        0    20021 2024-05-05 16:10:17.000000 funky_modifiers-0.1.8/src/funk_py/sorting/converters.py
+-rw-rw-rw-   0        0        0    19628 2024-05-07 11:15:54.000000 funky_modifiers-0.1.8/src/funk_py/sorting/dict_manip.py
+-rw-rw-rw-   0        0        0    18831 2024-05-09 11:15:54.000000 funky_modifiers-0.1.8/src/funk_py/sorting/pieces.py
+drwxrwxrwx   0        0        0        0 2024-05-09 11:17:07.542318 funky_modifiers-0.1.8/src/funk_py/super_dicts/
+-rw-rw-rw-   0        0        0     2139 2024-05-05 18:39:34.000000 funky_modifiers-0.1.8/src/funk_py/super_dicts/__init__.py
+-rw-rw-rw-   0        0        0     8330 2024-03-03 18:51:02.000000 funky_modifiers-0.1.8/src/funk_py/super_dicts/drop_none_dict.py
+-rw-rw-rw-   0        0        0     8942 2024-03-03 17:19:44.000000 funky_modifiers-0.1.8/src/funk_py/super_dicts/list_dict.py
+-rw-rw-rw-   0        0        0     3583 2023-12-30 12:27:19.000000 funky_modifiers-0.1.8/src/funk_py/super_dicts/windowed_list.py
+drwxrwxrwx   0        0        0        0 2024-05-09 11:17:07.564636 funky_modifiers-0.1.8/src/funky_modifiers.egg-info/
+-rw-rw-rw-   0        0        0      474 2024-05-09 11:17:07.000000 funky_modifiers-0.1.8/src/funky_modifiers.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1259 2024-05-09 11:17:07.000000 funky_modifiers-0.1.8/src/funky_modifiers.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-09 11:17:07.000000 funky_modifiers-0.1.8/src/funky_modifiers.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2024-05-09 11:17:07.000000 funky_modifiers-0.1.8/src/funky_modifiers.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-09 11:17:07.000000 funky_modifiers-0.1.8/src/funky_modifiers.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-09 11:17:07.563148 funky_modifiers-0.1.8/test/
+-rw-rw-rw-   0        0        0    21040 2024-05-03 11:33:03.000000 funky_modifiers-0.1.8/test/test_check_dict_equality.py
+-rw-rw-rw-   0        0        0    27490 2024-05-03 11:33:03.000000 funky_modifiers-0.1.8/test/test_check_list_equality.py
+-rw-rw-rw-   0        0        0    21911 2024-04-27 15:34:29.000000 funky_modifiers-0.1.8/test/test_convert_tuplish_dict.py
+-rw-rw-rw-   0        0        0    15212 2024-05-05 16:22:23.000000 funky_modifiers-0.1.8/test/test_converters.py
+-rw-rw-rw-   0        0        0     3127 2024-04-24 10:25:16.000000 funky_modifiers-0.1.8/test/test_converts_enums.py
+-rw-rw-rw-   0        0        0    12426 2024-03-03 19:25:27.000000 funky_modifiers-0.1.8/test/test_drop_none_dict.py
+-rw-rw-rw-   0        0        0    26544 2024-03-03 19:25:27.000000 funky_modifiers-0.1.8/test/test_function_hash_and_equality.py
+-rw-rw-rw-   0        0        0    12013 2024-04-12 20:31:58.000000 funky_modifiers-0.1.8/test/test_logs_vars.py
+-rw-rw-rw-   0        0        0    35329 2024-05-02 11:24:45.000000 funky_modifiers-0.1.8/test/test_obj.py
+-rw-rw-rw-   0        0        0    68867 2024-05-05 18:36:38.000000 funky_modifiers-0.1.8/test/test_pick.py
```

### Comparing `funky_modifiers-0.1.7/LICENSE` & `funky_modifiers-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.1.7/setup.py` & `funky_modifiers-0.1.8/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("requirements.txt", "r") as fh:
     install_requires = fh.read()
 
 setup(
     name='funky_modifiers',
-    version='0.1.7',
+    version='0.1.8',
     description='A package containing tiny bits and bobs to remove boilerplate or just make things simpler.',
     url='https://github.com/Sparqzi/funk_py',
     author='Erich Kopp',
     license='BSD 3-Clause',
     packages=find_packages(where='src'),
     package_dir={'': 'src'},
     classifiers=[
```

### Comparing `funky_modifiers-0.1.7/src/funk_py/modularity/basic_structures.py` & `funky_modifiers-0.1.8/src/funk_py/modularity/basic_structures.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.1.7/src/funk_py/modularity/bespoke_properties.py` & `funky_modifiers-0.1.8/src/funk_py/modularity/bespoke_properties.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.1.7/src/funk_py/modularity/decoration/enum_modifiers.py` & `funky_modifiers-0.1.8/src/funk_py/modularity/decoration/enum_modifiers.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.1.7/src/funk_py/modularity/decoration/init_modifiers.py` & `funky_modifiers-0.1.8/src/funk_py/modularity/decoration/init_modifiers.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.1.7/src/funk_py/modularity/decoration/transforming_list.py` & `funky_modifiers-0.1.8/src/funk_py/modularity/decoration/transforming_list.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.1.7/src/funk_py/modularity/logging.py` & `funky_modifiers-0.1.8/src/funk_py/modularity/logging.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.1.7/src/funk_py/modularity/type_matching.py` & `funky_modifiers-0.1.8/src/funk_py/modularity/type_matching.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.1.7/src/funk_py/sorting/converters.py` & `funky_modifiers-0.1.8/src/funk_py/sorting/converters.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.1.7/src/funk_py/sorting/dict_manip.py` & `funky_modifiers-0.1.8/src/funk_py/sorting/dict_manip.py`

 * *Files 2% similar despite different names*

```diff
@@ -415,12 +415,29 @@
         builder[str(key)].append(str(val))
 
     else:
         builder[str(key)] = [str(val)]
 
 
 def nest_under_keys(data: Any, *keys) -> dict:
+    """Generates a nested dictionary using ``keys`` as the nesting keys."""
     worker = data
     for key in reversed(keys):
         worker = {key: worker}
 
     return worker
+
+
+def get_subset(data: dict, *keys) -> dict:
+    """
+    Retrieves a subset of keys from a dictionary in the format of a dictionary. Any keys that do not
+    exist will simply be omitted.
+    """
+    return {key: data[key] for key in keys if key in data}
+
+
+def get_subset_values(data: dict, *keys) -> tuple:
+    """
+    Retireves a subset values (based on ``keys``) from a dictionary in the format of a tuple. Any
+    keys that do not exist will have ``None`` as their value.
+    """
+    return tuple(data.get(key, None) for key in keys)
```

### Comparing `funky_modifiers-0.1.7/src/funk_py/sorting/pieces.py` & `funky_modifiers-0.1.8/src/funk_py/sorting/pieces.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 import json
+from copy import deepcopy
 from enum import Enum
 from typing import Mapping, Any, Literal, Union, List, Tuple, Optional, Iterator, Generator, \
     Callable
 from urllib.parse import parse_qs
+
 import yaml
 
 from funk_py.modularity.decoration.enum_modifiers import converts_enums
 from funk_py.modularity.logging import make_logger
 from funk_py.sorting.converters import csv_to_json, xml_to_json, wonky_json_to_json, jsonl_to_json
-from funk_py.sorting.dict_manip import convert_tuplish_dict
+from funk_py.sorting.dict_manip import convert_tuplish_dict, get_subset_values, get_subset
 
 main_logger = make_logger('pieces', 'PIECES_LOG_LEVEL', default_level='warning')
 
 main_logger.info('Setting up simple types...')
 OutputMapSpecifier = Literal['json', 'jsonl', 'json\'',
                              'xml', 'xml-sa',
                              'e-list', 'list',
@@ -394,7 +396,114 @@
         args = args[0]
         if isinstance(args, dict):
             return convert_tuplish_dict(data, args.get('pair_name'),
                                         args.get('key_name'), args.get('val_name'))
 
         else:
             raise ValueError('TUPLE_DICT given an invalid argument format.')
+
+
+def fracture(
+        data: List[dict],
+        *keys: str,
+        inplace: bool = True
+) -> Generator[Tuple[dict, List[dict]], None, None]:
+    """
+    Separates a list of dictionaries into sets based on the values of a subset of keys and returns
+    each set one at a time.
+
+    :param data: The List to fracture.
+    :type data: List[dict]
+    :param keys: The subset of keys which should be used to differentiate between items in ``data``.
+    :type keys: str
+    :param inplace: Whether values returned should literally be the original values from the list or
+        should be copies of those values, set to ``False`` if you wish to avoid mutating the
+        original values in ``data``.
+    :type inplace: bool
+    :return: A ``Generator`` which iterates through each subset of ``data`` one at a time, basing
+        the subsets off of ``keys``.
+    """
+    # Choose the function we use to append values based on inplace.
+    # Choose it early since checking inplace inside the loop adds up on time.
+    if inplace:
+        def app_func(builder: List[dict], val: dict):
+            return builder.append(val)
+
+    else:
+        def app_func(builder: List[dict], val: dict):
+            return builder.append(deepcopy(val))
+
+    # Then just generate.
+    for subset in _iter_fracture(data, keys, app_func):
+        yield subset
+
+
+def _iter_fracture(
+        data: List[dict],
+        keys: Tuple[str, ...],
+        app_func: Callable[[List[dict], dict], None]
+) -> Generator[Tuple[dict, List[dict]], None, None]:
+    # The following two objects will be used to reduce repetitive calculations.
+    calc = [None] * len(data)
+    done = [False] * len(data)
+    for i, val in enumerate(data):
+        # Quite simply, don't generate a new list for something already included in a list.
+        if not done[i]:
+            builder = []
+            def1 = get_subset_values(val, *keys) if calc[i] is None else calc[i]
+            mark = get_subset(val, *keys)
+            app_func(builder, val)
+            for j, _val in enumerate(data)[i + 1:]:
+                if calc[j] is None:
+                    def2 = get_subset_values(_val, *keys) if calc[j] is None else calc[j]
+                    calc[j] = def2
+
+                else:
+                    def2 = calc[j]
+
+                if def1 == def2:
+                    app_func(builder, val)
+                    done[j] = True
+
+            yield mark, builder
+
+
+def translate(data: List[dict], translators: Mapping[Any, Callable[[dict], Any]],
+              default: Any = ..., inplace: bool = True) -> List[dict]:
+    """
+    Translate values in data based on given translators.
+
+    :param data: Dictionaries to translate.
+    :type data: List[dict]
+    :param translators: A dictionary of keys and functions used to translate values at those keys.
+    :type translators: Mapping[Any, Callable[[dict], Any]]
+    :param default: A default value to use for keys that don't exist. If this is not specified,
+        missing keys will simply be ignored.
+    :type default: Any
+    :param inplace: Whether to mutate ``data`` or not. Defaults to ``True``.
+    :type inplace: bool
+    :return: A list of the dictionaries in ``data`` mutated based on the functions in
+        ``translators``.
+    """
+    # Much more efficient to check inplace outside the loop.
+    if inplace:
+        for v in data:
+            for k, trans in translators.items():
+                if k in v:
+                    v[k] = trans(v[k])
+
+                elif default is not ...:
+                    v[k] = default
+
+        return data
+
+    output = []
+    for v in data:
+        output.append(builder := deepcopy(v))
+        for k, trans in translators.items():
+            if k in v:
+                builder[k] = trans(v[k])
+
+            elif default is not ...:
+                builder[k] = default
+
+    return output
```

### Comparing `funky_modifiers-0.1.7/src/funk_py/super_dicts/__init__.py` & `funky_modifiers-0.1.8/src/funk_py/super_dicts/__init__.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.1.7/src/funk_py/super_dicts/drop_none_dict.py` & `funky_modifiers-0.1.8/src/funk_py/super_dicts/drop_none_dict.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.1.7/src/funk_py/super_dicts/list_dict.py` & `funky_modifiers-0.1.8/src/funk_py/super_dicts/list_dict.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.1.7/src/funk_py/super_dicts/windowed_list.py` & `funky_modifiers-0.1.8/src/funk_py/super_dicts/windowed_list.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.1.7/src/funky_modifiers.egg-info/SOURCES.txt` & `funky_modifiers-0.1.8/src/funky_modifiers.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.1.7/test/test_check_dict_equality.py` & `funky_modifiers-0.1.8/test/test_check_dict_equality.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.1.7/test/test_check_list_equality.py` & `funky_modifiers-0.1.8/test/test_check_list_equality.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.1.7/test/test_convert_tuplish_dict.py` & `funky_modifiers-0.1.8/test/test_convert_tuplish_dict.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.1.7/test/test_converters.py` & `funky_modifiers-0.1.8/test/test_converters.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.1.7/test/test_converts_enums.py` & `funky_modifiers-0.1.8/test/test_converts_enums.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.1.7/test/test_drop_none_dict.py` & `funky_modifiers-0.1.8/test/test_drop_none_dict.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.1.7/test/test_function_hash_and_equality.py` & `funky_modifiers-0.1.8/test/test_function_hash_and_equality.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.1.7/test/test_logs_vars.py` & `funky_modifiers-0.1.8/test/test_logs_vars.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.1.7/test/test_obj.py` & `funky_modifiers-0.1.8/test/test_obj.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.1.7/test/test_pick.py` & `funky_modifiers-0.1.8/test/test_pick.py`

 * *Files identical despite different names*

