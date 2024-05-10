# Comparing `tmp/py-pane-0.8.1.tar.gz` & `tmp/py_pane-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-pane-0.8.1.tar", last modified: Sat Nov 18 19:40:40 2023, max compression
+gzip compressed data, was "py_pane-0.8.2.tar", last modified: Fri May 10 18:06:26 2024, max compression
```

## Comparing `py-pane-0.8.1.tar` & `py_pane-0.8.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-18 19:40:40.127382 py-pane-0.8.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2023-11-18 19:40:18.000000 py-pane-0.8.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5415 2023-11-18 19:40:40.127382 py-pane-0.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2993 2023-11-18 19:40:18.000000 py-pane-0.8.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-18 19:40:40.123382 py-pane-0.8.1/pane/
--rw-r--r--   0 runner    (1001) docker     (127)      718 2023-11-18 19:40:18.000000 py-pane-0.8.1/pane/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-18 19:40:40.123382 py-pane-0.8.1/pane/addons/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-18 19:40:18.000000 py-pane-0.8.1/pane/addons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2940 2023-11-18 19:40:18.000000 py-pane-0.8.1/pane/addons/numpy.py
--rw-r--r--   0 runner    (1001) docker     (127)     8311 2023-11-18 19:40:18.000000 py-pane-0.8.1/pane/annotations.py
--rw-r--r--   0 runner    (1001) docker     (127)    27163 2023-11-18 19:40:18.000000 py-pane-0.8.1/pane/classes.py
--rw-r--r--   0 runner    (1001) docker     (127)    11106 2023-11-18 19:40:18.000000 py-pane-0.8.1/pane/convert.py
--rw-r--r--   0 runner    (1001) docker     (127)    44146 2023-11-18 19:40:18.000000 py-pane-0.8.1/pane/converters.py
--rw-r--r--   0 runner    (1001) docker     (127)     8783 2023-11-18 19:40:18.000000 py-pane-0.8.1/pane/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     9453 2023-11-18 19:40:18.000000 py-pane-0.8.1/pane/field.py
--rw-r--r--   0 runner    (1001) docker     (127)     4845 2023-11-18 19:40:18.000000 py-pane-0.8.1/pane/types.py
--rw-r--r--   0 runner    (1001) docker     (127)    11151 2023-11-18 19:40:18.000000 py-pane-0.8.1/pane/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-18 19:40:40.127382 py-pane-0.8.1/py_pane.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5415 2023-11-18 19:40:40.000000 py-pane-0.8.1/py_pane.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      502 2023-11-18 19:40:40.000000 py-pane-0.8.1/py_pane.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-18 19:40:40.000000 py-pane-0.8.1/py_pane.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      149 2023-11-18 19:40:40.000000 py-pane-0.8.1/py_pane.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2023-11-18 19:40:40.000000 py-pane-0.8.1/py_pane.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1902 2023-11-18 19:40:18.000000 py-pane-0.8.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-18 19:40:40.127382 py-pane-0.8.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-18 19:40:40.127382 py-pane-0.8.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    13834 2023-11-18 19:40:18.000000 py-pane-0.8.1/tests/test_converters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2023-11-18 19:40:18.000000 py-pane-0.8.1/tests/test_field.py
--rw-r--r--   0 runner    (1001) docker     (127)     2568 2023-11-18 19:40:18.000000 py-pane-0.8.1/tests/test_numpy.py
--rw-r--r--   0 runner    (1001) docker     (127)     9489 2023-11-18 19:40:18.000000 py-pane-0.8.1/tests/test_pane.py
--rw-r--r--   0 runner    (1001) docker     (127)     1982 2023-11-18 19:40:18.000000 py-pane-0.8.1/tests/test_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     2583 2023-11-18 19:40:18.000000 py-pane-0.8.1/tests/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 18:06:26.532346 py_pane-0.8.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-10 18:06:13.000000 py_pane-0.8.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5533 2024-05-10 18:06:26.532346 py_pane-0.8.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2993 2024-05-10 18:06:13.000000 py_pane-0.8.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 18:06:26.528345 py_pane-0.8.2/pane/
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-05-10 18:06:13.000000 py_pane-0.8.2/pane/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 18:06:26.528345 py_pane-0.8.2/pane/addons/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 18:06:13.000000 py_pane-0.8.2/pane/addons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2962 2024-05-10 18:06:13.000000 py_pane-0.8.2/pane/addons/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8311 2024-05-10 18:06:13.000000 py_pane-0.8.2/pane/annotations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27235 2024-05-10 18:06:13.000000 py_pane-0.8.2/pane/classes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11485 2024-05-10 18:06:13.000000 py_pane-0.8.2/pane/convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44579 2024-05-10 18:06:13.000000 py_pane-0.8.2/pane/converters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8783 2024-05-10 18:06:13.000000 py_pane-0.8.2/pane/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9455 2024-05-10 18:06:13.000000 py_pane-0.8.2/pane/field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4845 2024-05-10 18:06:13.000000 py_pane-0.8.2/pane/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11122 2024-05-10 18:06:13.000000 py_pane-0.8.2/pane/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 18:06:26.532346 py_pane-0.8.2/py_pane.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5533 2024-05-10 18:06:26.000000 py_pane-0.8.2/py_pane.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-05-10 18:06:26.000000 py_pane-0.8.2/py_pane.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 18:06:26.000000 py_pane-0.8.2/py_pane.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-10 18:06:26.000000 py_pane-0.8.2/py_pane.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-10 18:06:26.000000 py_pane-0.8.2/py_pane.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1983 2024-05-10 18:06:13.000000 py_pane-0.8.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 18:06:26.532346 py_pane-0.8.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 18:06:26.528345 py_pane-0.8.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    13834 2024-05-10 18:06:13.000000 py_pane-0.8.2/tests/test_converters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-05-10 18:06:13.000000 py_pane-0.8.2/tests/test_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2568 2024-05-10 18:06:13.000000 py_pane-0.8.2/tests/test_numpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10004 2024-05-10 18:06:13.000000 py_pane-0.8.2/tests/test_pane.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1982 2024-05-10 18:06:13.000000 py_pane-0.8.2/tests/test_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2583 2024-05-10 18:06:13.000000 py_pane-0.8.2/tests/test_util.py
```

### Comparing `py-pane-0.8.1/LICENSE.txt` & `py_pane-0.8.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `py-pane-0.8.1/PKG-INFO` & `py_pane-0.8.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-pane
-Version: 0.8.1
+Version: 0.8.2
 Summary: A modern dataclass & data conversion library, focused on speed and expressiveness.
 Author-email: Colin Gilgenbach <hexane@mit.edu>
 License: MIT License
         
         Copyright (c) 2023 Colin Gilgenbach
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -22,14 +22,15 @@
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: Repository, https://github.com/hexane360/pane.git
+Project-URL: Documentation, https://hexane360.github.io/pane/
 Keywords: dataclass,validation,parsing,conversion
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -43,14 +44,15 @@
 Provides-Extra: dev
 Requires-Dist: pytest>=6.2.4; extra == "dev"
 Requires-Dist: numpy; extra == "dev"
 Provides-Extra: docs
 Requires-Dist: mkdocs>=1.5.2; extra == "docs"
 Requires-Dist: mkdocs-material==9.1.21; extra == "docs"
 Requires-Dist: mkdocstrings[python]==0.22.0; extra == "docs"
+Requires-Dist: markdown-include==0.8.1; extra == "docs"
 Requires-Dist: mike==1.1.2; extra == "docs"
 
 # pane
 
 `pane` is a modern Python library for dataclasses and data conversion, aiming
 for speed and expressiveness.
```

### Comparing `py-pane-0.8.1/README.md` & `py_pane-0.8.2/README.md`

 * *Files identical despite different names*

### Comparing `py-pane-0.8.1/pane/__init__.py` & `py_pane-0.8.2/pane/__init__.py`

 * *Files identical despite different names*

### Comparing `py-pane-0.8.1/pane/addons/numpy.py` & `py_pane-0.8.2/pane/addons/numpy.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 
     def _dtype_map(ty: t.Union[t.Type[t.Any], t.Type[generic]]) -> type:
         # TODO add a lookup table here
         # TODO add conditions to some types
         # e.g. unsigned int -> NonNegativeInt
         if ty in (_numpy.generic, _numpy.object_, t.Any):
-            return t.Any
+            return type(t.Any)
         if issubclass(ty, (_numpy.integer, int)):
             return int
         if issubclass(ty, (_numpy.floating, float)):
             return float
         if issubclass(ty, (_numpy.complexfloating, complex)):
             return complex
         if issubclass(ty, (_numpy.bool_, bool)):
@@ -56,15 +56,15 @@
                     raise TypeError(f"ndarray type argument should be 'numpy.dtype[<type>]', not '{dtype}'")
                 dtype = t.Any if len(dtype_args) < 1 else dtype_args[0]
         else:
             dtype = t.Any if len(args) < 1 else args[0]
 
         from ..converters import NestedSequenceConverter
 
-        return NestedSequenceConverter(dtype, array, ragged=False)
+        return NestedSequenceConverter(dtype, array, ragged=False)  # type: ignore
 
 except ImportError:
     if not t.TYPE_CHECKING:
         class generic():
             pass
 
         _DTypeScalar_co = t.TypeVar("_DTypeScalar_co", covariant=True, bound=generic)
```

### Comparing `py-pane-0.8.1/pane/annotations.py` & `py_pane-0.8.2/pane/annotations.py`

 * *Files identical despite different names*

### Comparing `py-pane-0.8.1/pane/classes.py` & `py_pane-0.8.2/pane/classes.py`

 * *Files 1% similar despite different names*

```diff
@@ -183,15 +183,15 @@
         import yaml
         try:
             from yaml import CSafeLoader as Loader
         except ImportError:
             from yaml import SafeLoader as Loader
 
         with open_file(f) as f:
-            obj = list(yaml.load_all(f, Loader))
+            obj: t.Any = list(yaml.load_all(f, Loader))  # type: ignore
 
         return cls.from_data(obj)
 
     @classmethod
     def from_yamls(cls, s: str) -> Self:
         """
         Load `cls` from a YAML string `s`
@@ -266,15 +266,15 @@
 
 @functools.lru_cache(maxsize=256)
 def _make_subclass(cls: t.Any, params: t.Tuple[t.Any, ...]) -> type:
     sup: t.Any = super(PaneBase, cls)
     if not hasattr(sup, '__class_getitem__'):
         raise TypeError(f"type '{cls}' is not subscriptable")
     alias: t.Type[PaneBase] = sup.__class_getitem__(params)  # type: ignore
-    typevars = getattr(cls, '__parameters__', ())
+    typevars: t.Tuple[Parameter, ...] = getattr(cls, '__parameters__', ())
 
     # return subclass with bound type variables
     bound_vars = dict(zip(typevars, params))
     return type(cls.__name__, (cls,), {
         PANE_BOUNDVARS: bound_vars,
         '__origin__': cls,
         '__parameters__': getattr(alias, '__parameters__'),
@@ -412,15 +412,15 @@
         # apply typevar replacements
         bound_vars = t.cast(t.Mapping[t.Union[t.TypeVar, ParamSpec], type], getattr(base, PANE_BOUNDVARS, {}))
         specs.update(cls_specs)
         specs = {k: spec.replace_typevars(bound_vars) for (k, spec) in specs.items()}
 
     annotations = get_type_hints(cls)
     kw_only = opts.kw_only  # current kw_only state
-    cls_specs = {}
+    cls_specs: t.Dict[str, FieldSpec] = {}
 
     for name, ty in annotations.items():
         if ty is KW_ONLY:
             # all further params are kw_only
             kw_only = True
             continue
```

### Comparing `py-pane-0.8.1/pane/convert.py` & `py_pane-0.8.2/pane/convert.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,19 +41,23 @@
 
         Any given type arguments are passed as positional arguments.
         This function should error when passed unknown type arguments.
         """
         ...
 
 
+ScalarType = t.Union[str, bytes, int, bool, float, complex, None]
+
 DataType = t.Union[str, bytes, int, bool, float, complex, None, t.Mapping['DataType', 'DataType'], t.Sequence['DataType'], numpy.NDArray[numpy.generic]]
 """Common data interchange type. [`into_data`][pane.convert.into_data] converts to this."""
 
-_DataType = (str, bytes, int, bool, float, complex, type(None), t.Mapping, t.Sequence, numpy.ndarray)  # type: ignore
-"""[`DataType`][pane.convert.DataType] for use in [`isinstance`][isinstance]."""
+_ScalarType = (str, bytes, int, bool, float, complex, type(None))  # type: ignore
+"""Scalar [`DataType`][pane.convert.DataType]s for use in [`isinstance`][isinstance] checks."""
+_DataType = (*_ScalarType, t.Mapping, t.Sequence, numpy.ndarray)  # type: ignore
+"""[`DataType`][pane.convert.DataType] for use in [`isinstance`][isinstance] checks."""
 
 Convertible = t.Union[
     DataType, HasConverter,
     t.AbstractSet[DataType],
     Fraction, Decimal,
     datetime.datetime, datetime.date, datetime.time,
     os.PathLike[str],
@@ -64,25 +68,25 @@
 Types supported by [`from_data`][pane.convert.from_data].
 
 Consists of [`DataType`][pane.convert.DataType] + [`HasConverter`][pane.convert.HasConverter] + supported stdlib types.
 """
 
 IntoConverter = t.Union[
     t.Type[Convertible],
-    t.Type[t.Any],
+    t.Any, t.Type[t.Any],
     t.Mapping[str, 'IntoConverter'],
     t.Sequence['IntoConverter']
 ]
 """
 Inputs supported by [`make_converter`][pane.convert.make_converter].
 Consists of `t.Type[Convertible]`, mappings (struct types), and sequences (tuple types).
 """
 
 
-_CONVERTER_HANDLERS: t.Sequence[t.Callable[[t.Any, t.Tuple[t.Any, ...]], Converter[t.Any]]] = []
+_CONVERTER_HANDLERS: t.List[t.Callable[[t.Any, t.Tuple[t.Any, ...]], Converter[t.Any]]] = []
 
 
 _ABSTRACT_MAPPING: t.Mapping[type, type] = t.cast(t.Mapping[type, type], {
     t.Sequence: tuple,
     collections.abc.Sequence: tuple,
     t.MutableSequence: list,
     collections.abc.MutableSequence: list,
@@ -116,17 +120,19 @@
     Supports types, mappings of types, and sequences of types.
     """
 
     from .converters import AnyConverter, StructConverter, SequenceConverter, UnionConverter
     from .converters import LiteralConverter, DictConverter, TupleConverter, ScalarConverter
     from .converters import EnumConverter, _BASIC_CONVERTERS, _BASIC_WITH_ARGS
 
-    if ty is t.Any:
+    if ty is t.Any or ty is type(t.Any):
         return AnyConverter()
     if isinstance(ty, t.TypeVar):
+        var_ty: IntoConverter
+
         if ty.__bound__ is not None:  # type: ignore
             # bound typevar
             var_ty = ty.__bound__
         elif len(ty.__constraints__) == 1:
             # typevar with constraints
             var_ty = ty.__constraints__
         elif len(ty.__constraints__) > 1:
@@ -218,15 +224,16 @@
     if issubclass(base, (dict, t.Mapping)):
         # map abstract to concrete types
         new_base = _ABSTRACT_MAPPING.get(base, base)  # type: ignore
         if inspect.isabstract(new_base):
             raise TypeError(f"No converter for abstract type '{ty}'")
         if issubclass(new_base, collections.Counter):
             # counter takes one type argument, handle it specially
-            return DictConverter(new_base, args[0] if len(args) > 0 else t.Any, int)
+            return DictConverter(new_base, # type: ignore
+                                 args[0] if len(args) > 0 else t.Any, int)
 
         # defaultdict needs a special constructor
         constructor: t.Optional[t.Callable[[t.Mapping[t.Any, t.Any]], collections.defaultdict[t.Any, t.Any]]]
         constructor = (lambda d: collections.defaultdict(None, d)) if issubclass(new_base, collections.defaultdict) else None
         return DictConverter(new_base,  # type: ignore
                              args[0] if len(args) > 0 else t.Any,
                              args[1] if len(args) > 1 else t.Any,
@@ -292,15 +299,16 @@
 
 
 def into_data(val: Convertible, ty: t.Optional[IntoConverter] = None) -> DataType:
     """
     Convert `val` of type `ty` into a data interchange format.
     """
     if ty is None:
-        if isinstance(val, _DataType):
+        if isinstance(val, _ScalarType):
+            # we can bypass the converter for scalar types
             return val
         ty = type(val)
 
     try:
         conv = make_converter(ty)
     except TypeError:
         raise TypeError(f"Can't convert type '{type(val)}' into data.") from None
```

### Comparing `py-pane-0.8.1/pane/converters.py` & `py_pane-0.8.2/pane/converters.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import re
 import traceback
 import datetime
 import enum
 from fractions import Fraction
 from decimal import Decimal
 import typing as t
-from typing_extensions import TypeGuard
+from typing_extensions import TypeGuard, TypeAlias
 
 from pane.errors import ErrorNode
 
 from .convert import DataType, Convertible, IntoConverter, make_converter, into_data
 from .util import list_phrase, pluralize, flatten_union_args, type_union, KW_ONLY
 from .errors import ConvertError, ParseInterrupt, WrongTypeError, ConditionFailedError
 from .errors import ErrorNode, SumErrorNode, ProductErrorNode
@@ -25,16 +25,17 @@
 
 T_co = t.TypeVar('T_co', covariant=True)
 T = t.TypeVar('T')
 U = t.TypeVar('U', bound=Convertible)
 FromDataT = t.TypeVar('FromDataT', bound=Convertible)
 FromDataK = t.TypeVar('FromDataK', bound=Convertible)
 FromDataV = t.TypeVar('FromDataV', bound=Convertible)
-NestedSequence = t.Union[T, t.Sequence['NestedSequence[T]']]
+NestedSequence: TypeAlias = t.Union[T, t.Sequence['NestedSequence[T]']]
 DatetimeT = t.TypeVar('DatetimeT', bound=t.Union[datetime.datetime, datetime.date, datetime.time])
+_ProductErrorChildren: TypeAlias = t.Dict[t.Union[int, str], ErrorNode]
 
 
 def data_is_sequence(val: t.Any) -> TypeGuard[t.Sequence[t.Any]]:
     """Return whether `val` is a sequence-like data type."""
     return isinstance(val, t.Sequence) and not isinstance(val, (str, bytes, bytearray))
 
 
@@ -151,15 +152,15 @@
                 raise ParseInterrupt()
         raise ParseInterrupt()
 
     def collect_errors(self, val: t.Any) -> t.Optional[WrongTypeError]:
         """See [`Converter.collect_errors`][pane.converters.Converter.collect_errors]"""
         if isinstance(val, self.allowed):
             try:
-                self.ty(val)
+                self.ty(val)  # type: ignore
                 return None
             except Exception as e:
                 tb = e.__traceback__.tb_next  # type: ignore
                 tb = traceback.TracebackException(type(e), e, tb)
                 return WrongTypeError(self.expected(), val, tb)
         return WrongTypeError(f'{self.expected()}', val)
 
@@ -513,15 +514,15 @@
         return None
 
 
 @dataclasses.dataclass(init=False)
 class TupleConverter(t.Generic[T], Converter[T]):
     """Converter for a simple, heterogeneous tuple-like type"""
     ty: t.Type[T]
-    """Type to convert into. Must be constructible from a sequence/tuple"""
+    """Type to convert into. Must be constructible from an iterable"""
     converters: t.Tuple[Converter[t.Any], ...]
     """List of sub-converters for each field"""
 
     def __init__(self, ty: t.Type[T], types: t.Sequence[IntoConverter]):
         self.ty = ty
         self.converters = tuple(map(make_converter, types))
 
@@ -539,21 +540,21 @@
     def try_convert(self, val: t.Any) -> T:
         """See [`Converter.try_convert`][pane.converters.Converter.try_convert]"""
         if not data_is_sequence(val):
             raise ParseInterrupt
         if len(val) != len(self.converters):
             raise ParseInterrupt
 
-        return self.ty(conv.try_convert(v) for (conv, v) in zip(self.converters, val))
+        return self.ty(conv.try_convert(v) for (conv, v) in zip(self.converters, val))  # type: ignore
 
     def collect_errors(self, val: t.Any) -> t.Union[None, ProductErrorNode, WrongTypeError]:
         """See [`Converter.collect_errors`][pane.converters.Converter.collect_errors]"""
         if not data_is_sequence(val) or len(val) != len(self.converters):
             return WrongTypeError(self.expected(), val)
-        children = {}
+        children: _ProductErrorChildren = {}
         for (i, (conv, v)) in enumerate(zip(self.converters, val)):
             node = conv.collect_errors(v)
             if node is not None:
                 children[i] = node
         if len(children) == 0:
             return None
         return ProductErrorNode(self.expected(), children, val)
@@ -567,15 +568,15 @@
     k_conv: Converter[FromDataK]
     """Sub-converter for keys"""
     v_conv: Converter[FromDataV]
     """Sub-converter for values"""
     constructor: t.Callable[[t.Dict[t.Any, t.Any]], t.Mapping[FromDataK, FromDataV]]
 
     def __init__(self, ty: t.Type[t.Dict[t.Any, t.Any]],
-                 k: t.Type[FromDataK] = t.Any, v: t.Type[FromDataV] = t.Any,
+                 k: t.Type[FromDataK] = type(t.Any), v: t.Type[FromDataV] = type(t.Any),
                  constructor: t.Optional[t.Callable[[t.Dict[t.Any, t.Any]], t.Mapping[FromDataK, FromDataV]]] = None):
         self.ty = ty
         self.k_conv = make_converter(k)
         self.v_conv = make_converter(v)
         self.constructor = self.ty if constructor is None else constructor
 
     def into_data(self, val: t.Any) -> DataType:
@@ -599,15 +600,15 @@
         return self.constructor(d)
 
     def collect_errors(self, val: t.Any) -> t.Union[None, WrongTypeError, ProductErrorNode]:
         """See [`Converter.collect_errors`][pane.converters.Converter.collect_errors]"""
         if not data_is_mapping(val):
             return WrongTypeError(self.expected(), val)
 
-        nodes: t.Dict[t.Union[str, int], ErrorNode] = {}
+        nodes: _ProductErrorChildren = {}
         for (k, v) in val.items():
             if (node := self.k_conv.collect_errors(k)) is not None:
                 nodes[str(k)] = node  # TODO split bad fields from bad values
             if (node := self.v_conv.collect_errors(v)) is not None:
                 nodes[str(k)] = node
         if len(nodes):
             return ProductErrorNode(self.expected(), nodes, val)
@@ -616,28 +617,30 @@
 @dataclasses.dataclass(init=False)
 class SequenceConverter(t.Generic[FromDataT], Converter[t.Sequence[FromDataT]]):
     """Converter for a homogenous sequence-like type"""
     ty: type
     """Type to convert into. Must be constructible from an iterator."""
     v_conv: Converter[FromDataT]
     """Sub-converter for values"""
-    constructor: t.Callable[[t.Iterator[t.Any]], t.Sequence[t.Any]]
+    constructor: t.Callable[[t.Iterable[t.Any]], t.Sequence[t.Any]]
 
-    def __init__(self, ty: t.Type[t.Sequence[t.Any]], v: t.Type[FromDataT] = t.Any,
-                 constructor: t.Optional[t.Callable[[t.Iterator[t.Any]], t.Sequence[t.Any]]] = None):
+    def __init__(self, ty: t.Type[t.Sequence[t.Any]], v: t.Type[FromDataT] = type(t.Any),
+                 constructor: t.Optional[t.Callable[[t.Iterable[t.Any]], t.Sequence[t.Any]]] = None):
         self.ty = ty
         self.v_conv = make_converter(v)
         self.constructor = self.ty if constructor is None else constructor
 
     def into_data(self, val: t.Any) -> DataType:
         """See [`Converter.into_data`][pane.converters.Converter.into_data]"""
-        return [
+        # construct tuple from a tuple, or a list otherwise
+        constructor = t.cast(t.Callable[[t.Iterable[t.Any]], t.Sequence[t.Any]], tuple if self.constructor is tuple else list)
+        return constructor(
             self.v_conv.into_data(v)
             for v in t.cast(t.Sequence[FromDataT], val)
-        ]
+        )
 
     def expected(self, plural: bool = False) -> str:
         """See [`Converter.expected`][pane.converters.Converter.expected]"""
         return f"{pluralize('sequence', plural)} of {self.v_conv.expected(True)}"
 
     def try_convert(self, val: t.Any) -> t.Sequence[FromDataT]:
         """See [`Converter.try_convert`][pane.converters.Converter.try_convert]"""
@@ -649,15 +652,15 @@
             raise ParseInterrupt()
 
     def collect_errors(self, val: t.Any) -> t.Union[None, WrongTypeError, ProductErrorNode]:
         """See [`Converter.collect_errors`][pane.converters.Converter.collect_errors]"""
         if not data_is_sequence(val):
             return WrongTypeError(self.expected(), val)
 
-        nodes = {}
+        nodes: t.Dict[t.Union[int, str], ErrorNode] = {}
         vals: t.List[FromDataT] = []
         for (i, v) in enumerate(val):
             try:
                 vals.append(self.v_conv.convert(v))
             except ConvertError as e:
                 nodes[i] = e.tree
 
@@ -743,15 +746,15 @@
             tb = e.__traceback__.tb_next  # type: ignore
             tb = traceback.TracebackException(type(e), e, tb)
             return WrongTypeError(self.expected(), val, tb)
 
     def _collect_errors(self, val: t.Any) -> t.Optional[ErrorNode]:
         if not data_is_sequence(val):
             return self.val_conv.collect_errors(val)
-        nodes = {}
+        nodes: _ProductErrorChildren = {}
         for (i, v) in enumerate(val):
             if (node := self._collect_errors(v)) is not None:
                 nodes[i] = node
         if len(nodes):
             return ProductErrorNode(self.expected(), nodes, val)
 
 
@@ -981,15 +984,15 @@
         datetime.time: "time",
     }
 
     def __init__(self, ty: t.Type[DatetimeT]):
         self.ty = ty
         self.super_ty: t.Type[DatetimeT]
         if ty in self._date_types:
-            self.super_ty = ty
+            self.super_ty = t.cast(t.Type[DatetimeT], ty)
             return
         for date_ty in self._date_types:
             if issubclass(ty, date_ty):
                 self.super_ty = t.cast(t.Type[DatetimeT], date_ty)
                 return
         raise TypeError(f"Only types {list_phrase([repr(str(ty)) for ty in self._date_types])} are supported")
```

### Comparing `py-pane-0.8.1/pane/errors.py` & `py_pane-0.8.2/pane/errors.py`

 * *Files identical despite different names*

### Comparing `py-pane-0.8.1/pane/field.py` & `py_pane-0.8.2/pane/field.py`

 * *Files 0% similar despite different names*

```diff
@@ -79,15 +79,15 @@
 
     Typically instantiated from a [`FieldSpec`][pane.field.FieldSpec].
     """
 
     _: KW_ONLY = dataclasses.field(init=False, repr=False, compare=False)
     name: str
     """Name of field"""
-    type: type
+    type: t.Any
     """Type of field. Must be [`Convertible`][pane.convert.Convertible]."""
     in_names: t.Sequence[str]
     """List of names which convert to this field."""
     out_name: str
     """Name this field converts into."""
     init: bool = True
     """Whether to add this field to __init__ methods (and conversion)"""
@@ -134,15 +134,15 @@
     """Whether to add this field to __init__ methods (and conversion)"""
     default: t.Union[t.Any, _Missing] = _MISSING
     """Default value for field"""
     default_factory: t.Optional[t.Callable[[], t.Any]] = None
     """Default value factory for field"""
     kw_only: bool = False
     """Whether field is keyword only"""
-    ty: t.Union[type, _Missing] = _MISSING
+    ty: t.Union[t.Any, _Missing] = _MISSING
     """Type of field, if known. Must be Convertible."""
 
     def __post_init__(self):
         if isinstance(self.aliases, str):
             self.aliases = [self.aliases]
 
     def replace_typevars(self, replacements: t.Mapping[t.Union[t.TypeVar, ParamSpec], t.Type[t.Any]]) -> Self:
```

### Comparing `py-pane-0.8.1/pane/types.py` & `py_pane-0.8.2/pane/types.py`

 * *Files identical despite different names*

### Comparing `py-pane-0.8.1/pane/util.py` & `py_pane-0.8.2/pane/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -298,15 +298,15 @@
                 self._root[KEY] = self._root[RESULT] = None
                 del self.cache[oldkey]
                 self.cache[key] = oldroot
             else:
                 last = self._root[PREV]
                 link = [last, self._root, key, result]
                 last[NEXT] = self._root[PREV] = self.cache[key] = link
-                self.full = (self.maxsize is not None and len(self.cache) >= self.maxsize)
+                self.full = (len(self.cache) >= self.maxsize)
         return result
 
 
 # TODO support maxsize
 def key_cache(key_f: t.Callable[[t.Any], t.Any] = id, *, maxsize: t.Optional[int] = None) -> t.Callable[[t.Callable[P, T]], KeyCache[P, T]]:
     def inner(f: t.Callable[P, T]) -> KeyCache[P, T]:
         return t.cast(KeyCache[P, T], functools.update_wrapper(KeyCache(f, key_f, maxsize), f))
```

### Comparing `py-pane-0.8.1/py_pane.egg-info/PKG-INFO` & `py_pane-0.8.2/py_pane.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-pane
-Version: 0.8.1
+Version: 0.8.2
 Summary: A modern dataclass & data conversion library, focused on speed and expressiveness.
 Author-email: Colin Gilgenbach <hexane@mit.edu>
 License: MIT License
         
         Copyright (c) 2023 Colin Gilgenbach
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -22,14 +22,15 @@
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: Repository, https://github.com/hexane360/pane.git
+Project-URL: Documentation, https://hexane360.github.io/pane/
 Keywords: dataclass,validation,parsing,conversion
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -43,14 +44,15 @@
 Provides-Extra: dev
 Requires-Dist: pytest>=6.2.4; extra == "dev"
 Requires-Dist: numpy; extra == "dev"
 Provides-Extra: docs
 Requires-Dist: mkdocs>=1.5.2; extra == "docs"
 Requires-Dist: mkdocs-material==9.1.21; extra == "docs"
 Requires-Dist: mkdocstrings[python]==0.22.0; extra == "docs"
+Requires-Dist: markdown-include==0.8.1; extra == "docs"
 Requires-Dist: mike==1.1.2; extra == "docs"
 
 # pane
 
 `pane` is a modern Python library for dataclasses and data conversion, aiming
 for speed and expressiveness.
```

### Comparing `py-pane-0.8.1/pyproject.toml` & `py_pane-0.8.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=51.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "py-pane"
-version = "0.8.1"
+version = "0.8.2"
 authors = [
 	{name = "Colin Gilgenbach", email = "hexane@mit.edu"},
 ]
 license = {file = "LICENSE.txt"}
 description = "A modern dataclass & data conversion library, focused on speed and expressiveness."
 readme = "README.md"
 keywords = ["dataclass", "validation", "parsing", "conversion"]
@@ -34,19 +34,21 @@
   'pytest >= 6.2.4',
   'numpy',  # for testing
 ]
 docs = [
   'mkdocs>=1.5.2',
   'mkdocs-material==9.1.21',
   'mkdocstrings[python]==0.22.0',
+  'markdown-include==0.8.1',
   'mike==1.1.2',
 ]
 
 [project.urls]
 Repository = "https://github.com/hexane360/pane.git"
+Documentation = "https://hexane360.github.io/pane/"
 
 [tool.setuptools]
 packages = [
   "pane",
   "pane.addons",
 ]
```

### Comparing `py-pane-0.8.1/tests/test_converters.py` & `py_pane-0.8.2/tests/test_converters.py`

 * *Files identical despite different names*

### Comparing `py-pane-0.8.1/tests/test_field.py` & `py_pane-0.8.2/tests/test_field.py`

 * *Files identical despite different names*

### Comparing `py-pane-0.8.1/tests/test_numpy.py` & `py_pane-0.8.2/tests/test_numpy.py`

 * *Files identical despite different names*

### Comparing `py-pane-0.8.1/tests/test_pane.py` & `py_pane-0.8.2/tests/test_pane.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,15 +42,15 @@
         y: int
 
     with pytest.raises(TypeError, match="Field 'z' is kw_only but mandatory. This is incompatible with the 'tuple' in_format."):
         class RequiredKwOnlyTuple(RequiredKwOnly, in_format='tuple'):
             ...
 
 
-class TestClass(pane.PaneBase, out_format='tuple'):
+class TestClass(pane.PaneBase, in_format=('tuple, struct'), out_format='tuple'):
     x: int = 3
     y: float = 5.
 
     __test__ = False
 
 
 @pytest.mark.parametrize(('args', 'result'), [
@@ -120,14 +120,20 @@
     y: int = 2
     _: pane.KW_ONLY
     w: int
 
     __test__ = False
 
 
+class NestedClass(pane.PaneBase, in_format=('tuple',), out_format='tuple'):
+    x: TestClass
+    y: int
+    z: TestClass
+
+
 @pytest.mark.parametrize(('cls', 'sig'), [
     (TestClass, '(x: int = 3, y: float = 5.0) -> None'),
     (TestClass2, '(x: int = 1, y: int = 2, *, z: int = 3, w: int = 4) -> None'),
     (TestClass3, '(*, x: int = 1, z: int = 3, y: int = 2, w: int) -> None'),
     (TestClassInherit, '(x: int = 3, y: float = 5.0, *, z: float = 3.0) -> None'),
     (TestClassInherit2, '(x: int = 3, y: float = 5.0, w: int = 4, *, z: float = 3.0) -> None'),
     (TestClassModifyFields, '(x: float = 9.0, y: float = 5.0, *, z: float = 3.0) -> None'),
@@ -151,15 +157,16 @@
     # extra fields
     (TestClass, {'x': 3, 'y': 5., 'zz': 5}, ProductErrorNode('struct TestClass', {}, {'x': 3, 'y': 5., 'zz': 5}, extra={'zz'})),
     # duplicate keys
     (TestClass2, {'x': 3, 'w': 3, 'W': 4}, ProductErrorNode('struct TestClass2', {'W': DuplicateKeyError('W', ('w', 'W', 'P'))}, {'x': 3, 'w': 3, 'W': 4})),
     # extra fields, allow_extra=True
     (TestClass3, {'x': 2, 'y': 3, 'w': 4, 'zz': 5}, TestClass3(x=2, y=3, w=4)),
     # missing fields
-    (TestClass3, {}, ProductErrorNode('struct TestClass3', {}, {}, missing={'w'}))
+    (TestClass3, {}, ProductErrorNode('struct TestClass3', {}, {}, missing={'w'})),
+    (NestedClass, ({'x': 2, 'y': 4.}, 10, {'x': 4, 'y': 8.}), NestedClass(x=TestClass(x=2, y=4.0), y=10, z=TestClass(x=4, y=8.0))),
 ])
 def test_pane_convert(cls, val, result):
     if isinstance(result, ErrorNode):
         with pytest.raises(pane.ConvertError) as e:
             pane.convert(val, cls)
         assert e.value.tree == result
     else:
@@ -167,17 +174,21 @@
 
 
 @pytest.mark.parametrize(('val', 'result'), [
     # out_format tuple
     (TestClass(x=3, y=5.), (3, 5.)),
     # out_format struct
     (TestClass2(x=3, w=3), {'x': 3, 'y': 2, 'w': 3, 'z': 3}),
+    (NestedClass(TestClass(2, 4.), 10, TestClass(4, 8.)), ((2, 4.), 10, (4, 8.))),
+    ({'x': 5, 'y': TestClass(2, 4.)}, {'x': 5, 'y': (2, 4.)}),
 ])
 def test_pane_into_data(val: pane.PaneBase, result: pane.DataType):
-    assert val.into_data() == result
+    if isinstance(val, pane.PaneBase):
+        assert val.into_data() == result
+    assert pane.into_data(val) == result
 
 
 T = t.TypeVar('T')
 U = t.TypeVar('U')
 
 
 class GenericPane(pane.PaneBase, t.Generic[T]):
```

### Comparing `py-pane-0.8.1/tests/test_types.py` & `py_pane-0.8.2/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `py-pane-0.8.1/tests/test_util.py` & `py_pane-0.8.2/tests/test_util.py`

 * *Files identical despite different names*

