# Comparing `tmp/simplelens-1.0.5.tar.gz` & `tmp/simplelens-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simplelens-1.0.5.tar", last modified: Tue Mar 28 18:16:02 2023, max compression
+gzip compressed data, was "simplelens-1.1.0.tar", last modified: Fri May 10 17:05:14 2024, max compression
```

## Comparing `simplelens-1.0.5.tar` & `simplelens-1.1.0.tar`

### file list

```diff
@@ -1,15 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 18:16:02.498376 simplelens-1.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-03-28 18:16:02.498376 simplelens-1.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-03-28 18:15:47.000000 simplelens-1.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 18:16:02.494376 simplelens-1.0.5/lens/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 18:15:47.000000 simplelens-1.0.5/lens/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5781 2023-03-28 18:15:47.000000 simplelens-1.0.5/lens/lens.py
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-03-28 18:15:47.000000 simplelens-1.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-28 18:16:02.498376 simplelens-1.0.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 18:16:02.498376 simplelens-1.0.5/simplelens.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-03-28 18:16:02.000000 simplelens-1.0.5/simplelens.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-03-28 18:16:02.000000 simplelens-1.0.5/simplelens.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-28 18:16:02.000000 simplelens-1.0.5/simplelens.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-03-28 18:16:02.000000 simplelens-1.0.5/simplelens.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 18:16:02.498376 simplelens-1.0.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     5110 2023-03-28 18:15:47.000000 simplelens-1.0.5/tests/test_lens.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 17:05:14.398829 simplelens-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1985 2024-05-10 17:05:14.398829 simplelens-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1783 2024-05-10 17:05:05.000000 simplelens-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 17:05:14.394829 simplelens-1.1.0/lens/
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-10 17:05:05.000000 simplelens-1.1.0/lens/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5896 2024-05-10 17:05:05.000000 simplelens-1.1.0/lens/lens.py
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-10 17:05:05.000000 simplelens-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 17:05:14.398829 simplelens-1.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 17:05:14.398829 simplelens-1.1.0/simplelens.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1985 2024-05-10 17:05:14.000000 simplelens-1.1.0/simplelens.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-05-10 17:05:14.000000 simplelens-1.1.0/simplelens.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 17:05:14.000000 simplelens-1.1.0/simplelens.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-10 17:05:14.000000 simplelens-1.1.0/simplelens.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-10 17:05:14.000000 simplelens-1.1.0/simplelens.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 17:05:14.398829 simplelens-1.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-10 17:05:05.000000 simplelens-1.1.0/tests/test_focus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5528 2024-05-10 17:05:05.000000 simplelens-1.1.0/tests/test_lens.py
```

### Comparing `simplelens-1.0.5/PKG-INFO` & `simplelens-1.1.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: simplelens
-Version: 1.0.5
+Version: 1.1.0
 Summary: Implementation of the lens functional pattern
+Requires-Python: >=3.11
 Description-Content-Type: text/markdown
+Requires-Dist: build==1.2.1
 
-# Lens
+# Lens v1.1.0
 
 ## Purpose
 
 The purpose of this project is to implement the "Lens" functional pattern in Python and supply that implementation as a package that can be imported into any other python project.
 
 
 ## Install
@@ -17,31 +19,31 @@
 
 ## Uninstall
 
     pip uninstall simplelens
 
 ## Usage
 Install the package from PyPi via pip install
-`from lens import lens`
+`from lens import focus`
 
 The lens function expects a collection of some form, as well as a list of keys and/or indexes to use to extract data 
 from the collection.
 
     collection = {'a': {'b': [{'a': 1}, {'b': 2}, {'c': 3}]
-    lens(collection, ['a', 'b', 2, 'c'])
+    focus(collection, ['a', 'b', 2, 'c'])
     #=> 3
 
 
 ## Changelog
   See changelog here: [Changelog.md](changelog.md)
 
 
 ## License
 
-Copyright 2023 Nathan Menge - nathan.menge@gmail.com
+Copyright 2024 Nathan Menge - nathan.menge@gmail.com
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
 documentation files (the "Software"), to deal in the Software without restriction, including without limitation the
 rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to
 permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all copies or substantial portions of the
```

### Comparing `simplelens-1.0.5/README.md` & `simplelens-1.1.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Lens
+# Lens v1.1.0
 
 ## Purpose
 
 The purpose of this project is to implement the "Lens" functional pattern in Python and supply that implementation as a package that can be imported into any other python project.
 
 
 ## Install
@@ -11,31 +11,31 @@
 
 ## Uninstall
 
     pip uninstall simplelens
 
 ## Usage
 Install the package from PyPi via pip install
-`from lens import lens`
+`from lens import focus`
 
 The lens function expects a collection of some form, as well as a list of keys and/or indexes to use to extract data 
 from the collection.
 
     collection = {'a': {'b': [{'a': 1}, {'b': 2}, {'c': 3}]
-    lens(collection, ['a', 'b', 2, 'c'])
+    focus(collection, ['a', 'b', 2, 'c'])
     #=> 3
 
 
 ## Changelog
   See changelog here: [Changelog.md](changelog.md)
 
 
 ## License
 
-Copyright 2023 Nathan Menge - nathan.menge@gmail.com
+Copyright 2024 Nathan Menge - nathan.menge@gmail.com
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
 documentation files (the "Software"), to deal in the Software without restriction, including without limitation the
 rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to
 permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all copies or substantial portions of the
```

### Comparing `simplelens-1.0.5/lens/lens.py` & `simplelens-1.1.0/lens/lens.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,70 +12,72 @@
 # WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS
 # OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR
 # OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 
 # This module is included as it is useful to this project and I wasn't ready to open source it, but hopefully I will do
 # that soon.  At which point I will remove this and pull it as a dependency through pip.
 
-from collections.abc import Iterable, Mapping, Sequence
+from collections.abc import Iterable, Mapping
 from functools import partial, reduce
-from typing import Any, cast, Dict, List, no_type_check, Optional, Tuple, Union
+from typing import Any, cast, Optional, Sequence
 
 
 def lens(collection: Iterable,
-         keys: List[Union[int, str, Tuple[str, Dict]]],
+         keys: Sequence,
          always_flatten: Optional[bool] = None) -> Any:
     """
     This function implements the "lens" functional pattern that is used to extract data from within complex
     data structures.
     A specific feature of this implementation that is perhaps atyipical, is that it only pulls values from Mappings and
     Objects.  When it encounters something List-like, it maps the current key across the list and pulls the values from
     the list elements up to the list.  It does not flatten the lists.
     :param collection: The collection to extract data from
     :type collection: Iterable
     :param keys: Keys used for extraction
-    :type keys: List[Union[int, str, Tuple[int, str, Dict]]
+    :type keys: List[Union[int, str, tuple[int, str, dict]]
     :param always_flatten: Flag to set flattening behavior across the entire function call
     :type always_flatten: bool
     :return: Returns data found within the data structure
     :rtype: Any
     """
     if always_flatten is None:
         always_flatten = True
     reducer = partial(_reducer, always_flatten=always_flatten)
     try:
         return reduce(reducer, keys, collection)
     except AttributeError as ae:
         msg = f"{ae}.\nAttempting to focus lens across key set {keys}"
         raise FocusingError(msg) from None
+    except IndexError:
+        raise FocusingError(f"Collection emptied while attempting to focus across key set: {keys}") from None
     except KeyError as ke:
         collection = cast(Mapping, collection)
         collection_key_list = list(collection.keys())
         joined_keys = ', '.join(collection_key_list)
         msg = (f"Could not find key {ke} in collection with keys '{joined_keys}'.\nAttempting to focus lens "
                f"across key set {keys}")
         raise FocusingError(msg) from None
 
 
-def _reducer(acc: Union[Mapping, Sequence], i: Union[int, str, Tuple], always_flatten: bool) -> Any:
+def _reducer(acc: Mapping | Sequence, i: int | str | tuple, always_flatten: bool) -> Any:
     """
     This is the reducer function for the lens.
     :param acc: The collection to reduce
     :type acc: Any
     :param i: The key to reduce the collection by, which in this case is to pull a value from the collection
     based on this value
-    :type i: Union[Dict, int, str, Tuple]
+    :type i: Union[dict, int, str, tuple]
     :return: Returns the focused result set, which can be almost anything
     :rtype: Any
     """
     j, args = unpack_element(i)
     force_map = args.get('force_map', False)
     flatten = force_map or args.get('flatten', always_flatten)
     if isinstance(acc, Mapping):
-        # It is a Mapping which implies Dict-like behavior
+        # It is a Mapping which implies dict-like behavior
         return acc[j]
     if isinstance(acc, Sequence) and not isinstance(acc, str):
         # It is a Sequence, which implies List-like behavior, but we keep out strings, which are also list-like
         if isinstance(j, int) and not force_map:
             return acc[j]
         mapped_list = list(map(lambda x: _reducer(x, j, always_flatten), acc))  # type: ignore
         if flatten:
@@ -85,32 +87,36 @@
         # It is neither a Mapping or Sequence, which only really leaves it as an attribute
         try:
             return getattr(acc, str(i))
         except AttributeError:
             raise AttributeError(f"Object with value '{acc}' has no attribute '{i}'") from None
 
 
-@no_type_check
-def unpack_element(element: Union[int, str, Tuple[Union[int, str], Dict]]) -> Tuple[Union[str, int], Dict]:
+def unpack_element(element: int | str | tuple[int | str, dict]) -> tuple[int | str, dict]:
     if isinstance(element, str):
         return element, {}
     if isinstance(element, int):
         return element, {}
     if isinstance(element, tuple):
-        try:
-            element, args = element  # type: ignore
-        except ValueError:
-            if len(element) < 2:
-                return element[0], {}
-            raise FocusingError(f"Unpacking a tuple: {element} that has more than 2 elements") from None
-        return element, args
+        return unpack_tuple(element)
     raise ValueError(f"Element {element} is not a str, int, or tuple[2] and is not supported")
 
 
-def _flatten(tall_list: List[List]) -> List:
+def unpack_tuple(element: tuple[int | str, dict]) -> tuple[int | str, dict]:
+    tuple_length = len(element)
+    if tuple_length == 2:
+        return element
+    if tuple_length == 1:
+        return element[0], {}
+    if tuple_length < 1:
+        raise ValueError('Element is an empty tuple')
+    raise ValueError(f"Unpacking a tuple: {element} that has more than 2 elements")
+
+
+def _flatten(tall_list: list[list]) -> list:
     """
     This method is used to flatten a single level of nested list.
     :param tall_list: List to flatten
     :return: List
     """
     return_val = []
     for el in tall_list:
@@ -119,9 +125,7 @@
         else:
             return_val.append(el)
     return return_val
 
 
 class FocusingError(Exception):
     pass
-
-# pylama:ignore=C901
```

### Comparing `simplelens-1.0.5/simplelens.egg-info/PKG-INFO` & `simplelens-1.1.0/simplelens.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: simplelens
-Version: 1.0.5
+Version: 1.1.0
 Summary: Implementation of the lens functional pattern
+Requires-Python: >=3.11
 Description-Content-Type: text/markdown
+Requires-Dist: build==1.2.1
 
-# Lens
+# Lens v1.1.0
 
 ## Purpose
 
 The purpose of this project is to implement the "Lens" functional pattern in Python and supply that implementation as a package that can be imported into any other python project.
 
 
 ## Install
@@ -17,31 +19,31 @@
 
 ## Uninstall
 
     pip uninstall simplelens
 
 ## Usage
 Install the package from PyPi via pip install
-`from lens import lens`
+`from lens import focus`
 
 The lens function expects a collection of some form, as well as a list of keys and/or indexes to use to extract data 
 from the collection.
 
     collection = {'a': {'b': [{'a': 1}, {'b': 2}, {'c': 3}]
-    lens(collection, ['a', 'b', 2, 'c'])
+    focus(collection, ['a', 'b', 2, 'c'])
     #=> 3
 
 
 ## Changelog
   See changelog here: [Changelog.md](changelog.md)
 
 
 ## License
 
-Copyright 2023 Nathan Menge - nathan.menge@gmail.com
+Copyright 2024 Nathan Menge - nathan.menge@gmail.com
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
 documentation files (the "Software"), to deal in the Software without restriction, including without limitation the
 rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to
 permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all copies or substantial portions of the
```

### Comparing `simplelens-1.0.5/tests/test_lens.py` & `simplelens-1.1.0/tests/test_lens.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,13 @@
-from lens import lens
 from pytest import fixture, mark, raises
 
 
+from lens import lens
+
+
 @fixture
 def complex_data_struct(list_based_struct):
     return {'a': 'aye', 'b_list': ['be', 'bee'],
             'c_list': [{'starts_with_c': ['cee', 'ce'], 'starts_with_s': ['see', 'sea']}],
             'nested_lists': [{'letters': ['a', 'b', 'c']}, {'letters': ['d', 'e', 'f']}, {'letters': ['g', 'h', 'i']},
                              {'letters': ['j', 'k', 'l']}, {'letters': ['m', 'n', 'o']}],
             'deeper_nest': list_based_struct}
@@ -120,21 +122,41 @@
 
 
 def test_lens_with_too_deep_key_chain(structure_with_objects):
     with raises(lens.FocusingError):
         lens.lens(structure_with_objects, ['object', 'yolo', 'word', 'more', 'i', 'want', 'more'])
 
 
+def test_lens_empty_list():
+    with raises(lens.FocusingError):
+        lens.lens([], [0, 'something'])
+
+
+def test_lens_empty_dict():
+    with raises(lens.FocusingError):
+        lens.lens({}, ['a', 'something'])
+
+
+def test_lens_empty_tuple():
+    with raises(lens.FocusingError):
+        lens.lens(tuple(), [0, 'thing'])
+
+
 @mark.parametrize('value,result', [(3, (3, {})), ('a', ('a', {})), (('yolo', {}), ('yolo', {})), (('a',), ('a', {})),
                                    ('id', ('id', {}))])
 def test_unpack_element(result, value):
     assert lens.unpack_element(value) == result
 
 
 def test_unpack_element_dict():
     with raises(ValueError):
         lens.unpack_element({'a': 'aye'})
 
 
 def test_unpack_element_oversized_tuple():
-    with raises(lens.FocusingError):
+    with raises(ValueError):
         lens.unpack_element(('yolo', 3, 2))
+
+
+def test_unpack_empty_tuple():
+    with raises(ValueError):
+        lens.unpack_element(tuple())
```

