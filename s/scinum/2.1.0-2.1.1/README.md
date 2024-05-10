# Comparing `tmp/scinum-2.1.0.tar.gz` & `tmp/scinum-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scinum-2.1.0.tar", last modified: Mon Mar 11 12:52:15 2024, max compression
+gzip compressed data, was "scinum-2.1.1.tar", last modified: Fri May 10 09:08:40 2024, max compression
```

## Comparing `scinum-2.1.0.tar` & `scinum-2.1.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 12:52:15.397012 scinum-2.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-03-11 12:51:55.000000 scinum-2.1.0/.flake8
--rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-03-11 12:51:55.000000 scinum-2.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-03-11 12:51:55.000000 scinum-2.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    14540 2024-03-11 12:52:15.397012 scinum-2.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10294 2024-03-11 12:51:55.000000 scinum-2.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1871 2024-03-11 12:51:57.000000 scinum-2.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-03-11 12:51:57.000000 scinum-2.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-03-11 12:51:57.000000 scinum-2.1.0/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-03-11 12:51:57.000000 scinum-2.1.0/requirements_docs.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 12:52:15.393012 scinum-2.1.0/scinum/
--rw-r--r--   0 runner    (1001) docker     (127)   101887 2024-03-11 12:51:57.000000 scinum-2.1.0/scinum/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 12:52:15.397012 scinum-2.1.0/scinum.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14540 2024-03-11 12:52:15.000000 scinum-2.1.0/scinum.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-03-11 12:52:15.000000 scinum-2.1.0/scinum.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-11 12:52:15.000000 scinum-2.1.0/scinum.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      492 2024-03-11 12:52:15.000000 scinum-2.1.0/scinum.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-11 12:52:15.000000 scinum-2.1.0/scinum.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-11 12:52:15.401012 scinum-2.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:08:40.464491 scinum-2.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-10 09:08:29.000000 scinum-2.1.1/.flake8
+-rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-05-10 09:08:29.000000 scinum-2.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-10 09:08:29.000000 scinum-2.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    14540 2024-05-10 09:08:40.464491 scinum-2.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10294 2024-05-10 09:08:29.000000 scinum-2.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1871 2024-05-10 09:08:29.000000 scinum-2.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-10 09:08:29.000000 scinum-2.1.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-10 09:08:29.000000 scinum-2.1.1/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-10 09:08:29.000000 scinum-2.1.1/requirements_docs.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:08:40.460491 scinum-2.1.1/scinum/
+-rw-r--r--   0 runner    (1001) docker     (127)   102490 2024-05-10 09:08:29.000000 scinum-2.1.1/scinum/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:08:40.460491 scinum-2.1.1/scinum.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14540 2024-05-10 09:08:40.000000 scinum-2.1.1/scinum.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-10 09:08:40.000000 scinum-2.1.1/scinum.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 09:08:40.000000 scinum-2.1.1/scinum.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2024-05-10 09:08:40.000000 scinum-2.1.1/scinum.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-10 09:08:40.000000 scinum-2.1.1/scinum.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 09:08:40.464491 scinum-2.1.1/setup.cfg
```

### Comparing `scinum-2.1.0/LICENSE` & `scinum-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `scinum-2.1.0/PKG-INFO` & `scinum-2.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scinum
-Version: 2.1.0
+Version: 2.1.1
 Summary: Scientific numbers with multiple uncertainties and correlation-aware, gaussian propagation and Numpy support.
 Author-email: Marcel Rieger <marcel.rieger@cern.ch>
 License: Copyright (c) 2017-2024, Marcel Rieger
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
```

### Comparing `scinum-2.1.0/README.md` & `scinum-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `scinum-2.1.0/pyproject.toml` & `scinum-2.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `scinum-2.1.0/scinum/__init__.py` & `scinum-2.1.1/scinum/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,26 +9,27 @@
 
 __author__ = "Marcel Rieger"
 __copyright__ = "Copyright 2017-2024, Marcel Rieger"
 __credits__ = ["Marcel Rieger"]
 __contact__ = "https://github.com/riga/scinum"
 __license__ = "BSD-3-Clause"
 __status__ = "Production/Stable"
-__version__ = "2.1.0"
+__version__ = "2.1.1"
 __all__ = [
     "Number", "Correlation", "DeferredResult", "Operation",
     "ops", "style_dict",
-    "NOMINAL", "UP", "DOWN", "N", "U", "D",
+    "NOMINAL", "UP", "DOWN", "DEFAULT", "ALL",
 ]
 
 import math
 import re
 import functools
 import operator
 import types
+import enum
 import decimal
 from collections import defaultdict
 from types import ModuleType
 from typing import TypeVar, Callable, Any, Sequence, Tuple, Dict, Union
 
 T = TypeVar("T")
 
@@ -166,14 +167,63 @@
         Build and returns the property's *fdel* method for the member defined by *name*.
         """
         def fdel(inst: typed) -> None:
             delattr(inst, name)
         return fdel
 
 
+class UncertaintyDirection(enum.Enum):
+    """
+    Enumeration of uncertainty directions.
+    """
+
+    NOMINAL = "nominal"
+    UP = "up"
+    DOWN = "down"
+
+    @classmethod
+    def check(cls, other: Any) -> bool:
+        return other in (cls.NOMINAL, cls.UP, cls.DOWN)
+
+    def __str__(self) -> str:
+        return self.value
+
+    def __eq__(self, other: Any) -> bool:
+        return str(self) == other
+
+    def __hash__(self) -> int:
+        return hash(self.value)
+
+
+class UncertaintyFlag(enum.Enum):
+    """
+    Enumeration of uncertainty flags.
+    """
+
+    DEFAULT = "default"
+    ALL = "all"
+
+    def __str__(self) -> str:
+        return self.value
+
+    def __eq__(self, other: Any) -> bool:
+        return str(self) == other
+
+    def __hash__(self) -> int:
+        return hash(self.value)
+
+
+# shorthands
+NOMINAL = UncertaintyDirection.NOMINAL
+UP = UncertaintyDirection.UP
+DOWN = UncertaintyDirection.DOWN
+DEFAULT = UncertaintyFlag.DEFAULT
+ALL = UncertaintyFlag.ALL
+
+
 class Number(object):
     """ __init__(nominal=0.0, uncertainties={})
     Implementation of a scientific number, i.e., a *nominal* value with named *uncertainties*.
     *uncertainties* should be a dict or convertable to a dict with strings as keys, and the
     corresponding uncertainties as values. Whereas different formats are accepted for values to
     denote whether the passed value is relative or absolute, it should be noted that after some
     initial parsing, they are always stored as absolute numbers represented by floats internally.
@@ -263,62 +313,14 @@
     .. py:classattribute:: default_style
 
         type: string
 
         The default style name (``"plain"``) that is used in :py:meth:`str()` when no style argument
         was passed.
 
-    .. py:classattribute:: DEFAULT
-
-        type: string
-
-        Constant that denotes the default uncertainty (``"default"``).
-
-    .. py:classattribute:: ALL
-
-        type: string
-
-        Constant that denotes all uncertainties (``"all"``).
-
-    .. py:classattribute:: NOMINAL
-
-        type: string
-
-        Constant that denotes the nominal value (``"nominal"``).
-
-    .. py:classattribute:: UP
-
-        type: string
-
-        Constant that denotes the up direction (``"up"``).
-
-    .. py:classattribute:: DOWN
-
-        type: string
-
-        Constant that denotes the down direction (``"down"``).
-
-    .. py:classattribute:: N
-
-        type: string
-
-        Shorthand for :py:attr:`NOMINAL`.
-
-    .. py:classattribute:: U
-
-        type: string
-
-        Shorthand for :py:attr:`UP`.
-
-    .. py:classattribute:: D
-
-        type: string
-
-        Shorthand for :py:attr:`DOWN`.
-
     .. py:attribute:: nominal
 
         type: float
 
         The nominal value.
 
     .. py:attribute:: n
@@ -349,27 +351,20 @@
 
         type: type
 
         The default dtype to use when a NumPy array is wrapped. The initial value is
         ``numpy.float32`` when NumPy is available, *None* otherwise.
     """
 
-    # uncertainty flags
-    DEFAULT = "default"
-    ALL = "all"
-
-    # uncertainty directions
-    NOMINAL = "nominal"
-    UP = "up"
-    DOWN = "down"
-
-    # aliases
-    N = NOMINAL
-    U = UP
-    D = DOWN
+    # uncertainty directions and flags for backwards compatibility
+    NOMINAL = UncertaintyDirection.NOMINAL
+    UP = UncertaintyDirection.UP
+    DOWN = UncertaintyDirection.DOWN
+    DEFAULT = UncertaintyFlag.DEFAULT
+    ALL = UncertaintyFlag.ALL
 
     default_format: str | int = "%s"
     default_style = "plain"
 
     def __init__(
         self,
         nominal: InValueType = 0.0,
@@ -452,14 +447,17 @@
             try:
                 uncertainties = dict(uncertainties)  # type: ignore[arg-type]
             except:
                 uncertainties = {self.DEFAULT: uncertainties}  # type: ignore[dict-item]
 
         _uncertainties: OutUncsType = {}
         for name, val in uncertainties.items():
+            if isinstance(name, UncertaintyFlag):
+                name = str(name)
+
             # check the name
             if not isinstance(name, str):
                 raise TypeError(f"invalid uncertainty name: {name}")
 
             # parse the value type
             if isinstance(val, (int, float, complex)) or is_numpy(val):
                 val = (val, val)  # type: ignore[assignment]
@@ -516,82 +514,83 @@
 
             _uncertainties[str(name)] = (up, down)  # type: ignore[assignment]
 
         return _uncertainties
 
     def get_uncertainty(
         self,
-        name: str = DEFAULT,
-        direction: str = NOMINAL,
+        name: UncertaintyFlag | str = UncertaintyFlag.DEFAULT,
+        direction: UncertaintyDirection | str = UncertaintyDirection.NOMINAL,
         *,
         default: T | None = None,
     ) -> OutValueType | OutUncType | T:
         """
         Returns the *absolute* up and down variaton in a 2-tuple for an uncertainty *name*. When
         *direction* is set, the particular value is returned instead of a 2-tuple. In case no
         uncertainty was found and *default* is not *None*, that value is returned.
         """
-        if direction not in (self.UP, self.DOWN, self.NOMINAL):
-            raise ValueError(f"unknown direction: {direction}")
+        if isinstance(name, UncertaintyFlag):
+            name = str(name)
+        direction = UncertaintyDirection(direction)
 
         if name not in self.uncertainties:
             if default is not None:
                 return default
             raise KeyError(f"no uncertainty '{name}' in {self!r}")
 
         unc = self.uncertainties[name]
 
         if direction == self.NOMINAL:
             return unc
 
-        return unc[0 if direction == self.UP else 1]
+        return unc[0 if direction == UncertaintyDirection.UP else 1]
 
     def u(
         self,
-        name: str = DEFAULT,
-        direction: str = NOMINAL,
+        name: UncertaintyFlag | str = UncertaintyFlag.DEFAULT,
+        direction: UncertaintyDirection | str = UncertaintyDirection.NOMINAL,
         *,
         default: T | None = None,
     ) -> OutValueType | OutUncType | T:
         """
         Shorthand for :py:meth:`get_uncertainty`.
         """
         return self.get_uncertainty(name=name, direction=direction, default=default)
 
     def set_uncertainty(
         self,
-        name: str,
+        name: UncertaintyFlag | str,
         value: InValueType | InUncType,
     ) -> None:
         """
         Sets the uncertainty *value* for an uncertainty *name*. *value* should have one of the
         formats as described in :py:meth:`uncertainties`.
         """
         uncertainties = self.__class__.uncertainties.fparse(self, {name: value})
         self._uncertainties.update(uncertainties)
 
     def combine_uncertaintes(
         self,
-        combine: str | dict[str, Sequence[str]] = ALL,
+        combine: UncertaintyFlag | str | dict[str, Sequence[str]] = UncertaintyFlag.ALL,
     ) -> Number:
         """ combine_uncertaintes(combine_uncs=ALL)
         Returns a copy of this number with certain uncertainties combined. *combine* can be a
         dictionary of keys mapping to strings denoting uncertainties that should be combined with
         keys refering to new names of the combined uncertainties.
 
         When :py:attr:`ALL`, all uncertainties are combined.
         """
         # create a map that contains all uncertainties
         combine_map: dict[str, list[str] | None] = {}
-        if combine == self.ALL:
-            combine_map[self.DEFAULT] = list(self.uncertainties.keys())
+        if combine == UncertaintyFlag.ALL:
+            combine_map[str(UncertaintyFlag.DEFAULT)] = list(self.uncertainties.keys())
         elif isinstance(combine, dict):
             seen_uncs: set = set()
             for new_name, names in combine.items():
-                if names == self.ALL:
+                if names == UncertaintyFlag.ALL:
                     combine_map[new_name] = list(self.uncertainties.keys())
                 elif isinstance(names, (list, tuple)):
                     combine_map[new_name] = list(names)
                 else:
                     raise ValueError(f"expected uncertainty names sequence, got '{names}'")
                 seen_uncs |= set(combine_map[new_name])  # type: ignore[arg-type]
             # add remaining uncertainties
@@ -603,15 +602,19 @@
 
         # create combined uncertainties
         uncs = {}
         for new_name, _names in combine_map.items():
             uncs[new_name] = (
                 self.uncertainties[new_name]
                 if _names is None
-                else self.get(direction=(self.UP, self.DOWN), names=_names, unc=True)
+                else self.get(
+                    direction=(UncertaintyDirection.UP, UncertaintyDirection.DOWN),
+                    names=_names,
+                    unc=True,
+                )
             )
 
         return self.__class__(self.nominal, uncs, **self._init_kwargs())  # type: ignore[arg-type]
 
     def clear(
         self,
         nominal: InValueType | None = None,
@@ -628,15 +631,15 @@
             self.nominal = nominal
         if uncertainties is not None:
             self.uncertainties = uncertainties
 
     def str(
         self,
         format: str | int | None = None,
-        combine_uncs: str | dict[str, Sequence[str]] | None = None,
+        combine_uncs: UncertaintyFlag | str | dict[str, Sequence[str]] | None = None,
         unit: str | None = None,
         scientific: bool = False,
         si: bool = False,
         labels: bool = True,
         style: str | None = None,
         styles: dict[str, str] | None = None,
         force_asymmetric: bool = False,
@@ -671,15 +674,15 @@
         .. code-block:: python
 
             n = Number(17.321, {"a": 1.158, "b": 0.453})
             n.str()                    # -> '17.321 +-1.158 (a) +-0.453 (b)'
             n.str("%.1f")              # -> '17.3 +-1.2 (a) +-0.5 (b)'
             n.str("publication")       # -> '17.32 +-1.16 (a) +-0.45 (b)'
             n.str("pdg")               # -> '17.3 +-1.2 (a) +-0.5 (b)'
-            n.str(combine_uncs="all")  # -> 'TODO'
+            n.str(combine_uncs="all")  # -> '17.321 +-1.2434520497389514'
 
             n = Number(8848, 10)
             n.str(unit="m")                           # -> "8848.0 +-10.0 m"
             n.str(unit="m", force_asymmetric=True)    # -> "8848.0 +10.0-10.0 m"
             n.str(unit="m", scientific=True)          # -> "8.848 +-0.01 x 1E3 m"
             n.str("%.2f", unit="m", scientific=True)  # -> "8.85 +-0.01 x 1E3 m"
             n.str(unit="m", si=True)                  # -> "8.848 +-0.01 km"
@@ -837,58 +840,60 @@
         if uncertainties is None:
             uncertainties = self.uncertainties
 
         return self.__class__(nominal, uncertainties=uncertainties)
 
     def get(
         self,
-        direction: str | tuple[str] = NOMINAL,
-        names: str | Sequence[str] = ALL,
+        direction:
+            UncertaintyDirection | str |
+            tuple[UncertaintyDirection | str, UncertaintyDirection | str] = UncertaintyDirection.NOMINAL,  # noqa
+        names: UncertaintyFlag | str | Sequence[str] = UncertaintyFlag.ALL,
         unc: bool = False,
         factor: bool = False,
     ) -> OutValueType | OutUncType:
         """
         Returns different representations of the contained value(s). *direction* should be any of
         *NOMINAL*, *UP* or *DOWN*, or a tuple containing a combination of them. When not *NOMINAL*,
         *names* decides which uncertainties to take into account for the combination. When *unc* is
         *True*, only the unsigned, combined uncertainty is returned. When *False*, the nominal value
         plus or minus the uncertainty is returned. When *factor* is *True*, the ratio w.r.t. the
         nominal value is returned.
         """
         if (
             isinstance(direction, tuple) and
-            all(d in (self.NOMINAL, self.UP, self.DOWN) for d in direction)  # type: ignore[union-attr] # noqa
+            all(UncertaintyDirection.check(d) for d in direction)  # type: ignore[union-attr]
         ):
             return tuple(  # type: ignore[return-value]
                 self.get(direction=d, names=names, unc=unc, factor=factor)
                 for d in direction  # type: ignore[union-attr]
             )
 
-        if direction == self.NOMINAL:
+        if direction == UncertaintyDirection.NOMINAL:
             value = self.nominal
 
-        elif direction in (self.UP, self.DOWN):
+        elif direction in (UncertaintyDirection.UP, UncertaintyDirection.DOWN):
             # find uncertainties to take into account
-            if names == self.ALL:
-                names = self.uncertainties.keys()
+            if names == UncertaintyFlag.ALL:
+                _names = self.uncertainties.keys()
             else:
-                names = make_list(names)
-                if any(name not in self.uncertainties for name in names):
-                    unknown = list(set(names) - set(self.uncertainties.keys()))
+                _names = make_list(names)
+                if any(name not in self.uncertainties for name in _names):
+                    unknown = list(set(_names) - set(self.uncertainties.keys()))
                     raise ValueError(f"unknown uncertainty name(s): {unknown}")
 
             # calculate the combined uncertainty without correlation
-            idx = int(direction == self.DOWN)
-            uncs = [self.uncertainties[name][idx] for name in names]
+            idx = int(direction == UncertaintyDirection.DOWN)
+            uncs = [self.uncertainties[name][idx] for name in _names]
             combined_unc = sum(u**2.0 for u in uncs)**0.5
 
             # determine the output value
             if unc:
                 value = combined_unc
-            elif direction == self.UP:
+            elif direction == UncertaintyDirection.UP:
                 value = self.nominal + combined_unc
             else:
                 value = self.nominal - combined_unc
 
         else:
             raise ValueError(f"unknown direction: {direction}")
 
@@ -1096,16 +1101,16 @@
             out.clear(result.nominal, result.uncertainties)
             result = out
 
         return result
 
     def __call__(
         self,
-        direction: str = NOMINAL,
-        names: str | Sequence[str] = ALL,
+        direction: UncertaintyDirection | str = UncertaintyDirection.NOMINAL,
+        names: UncertaintyFlag | str | Sequence[UncertaintyFlag | str] = UncertaintyFlag.ALL,
         unc: bool = False,
         factor: bool = False,
     ) -> OutValueType | OutUncType:
         # shorthand for get
         return self.get(direction=direction, names=names, unc=unc, factor=factor)
 
     def __float__(self) -> OutValueType:
@@ -1277,23 +1282,14 @@
 
         return ensure_number(other).pow(self, inplace=False)
 
     def __ipow__(self, other: Number | DeferredResult | InValueType) -> Number | DeferredResult:
         return self.pow(other, inplace=True)
 
 
-# module-wide shorthands for Number flags
-NOMINAL = Number.NOMINAL
-UP = Number.UP
-DOWN = Number.DOWN
-N = Number.N
-U = Number.U
-D = Number.D
-
-
 class Correlation(object):
     """ Correlation([default], **rhos)
     Container class describing correlations to be applied to equally named uncertainties when
     combining two :py:class:`Number` instances through an operator.
 
     A correlation object is therefore applied to a number by means of multiplication or matrix
     multiplication (i.e. ``*`` or ``@``), resulting in a :py:class:`DeferredResult` object which is
@@ -1980,27 +1976,14 @@
 
 
 @atanh.derive
 def atanh(x: Number | float | NDArray) -> Number | float | NDArray:
     return 1.0 / (1.0 - x**2.0)
 
 
-@ops.register(name="abs", ufuncs=["abs", "absolute"])
-def abs_op(x: Number | float | NDArray) -> Number | float | NDArray:
-    """ abs(x)
-    Absolute value function.
-    """
-    return infer_math(x).abs(x)
-
-
-@abs_op.derive
-def abs_op(x: Number | float | NDArray) -> Number | float | NDArray:
-    return infer_math(x).abs(x)  # TODO: this is not correct! do not commit
-
-
 #
 # helper functions
 #
 
 def try_float(x: Any) -> float | None:
     """
     Tries to convert a value *x* to float and returns it on success, and *None* otherwise.
@@ -2040,27 +2023,27 @@
     ``ufloat``.
     """
     return HAS_UNCERTAINTIES and isinstance(x, _uncs.core.AffineScalarFunc)
 
 
 def parse_ufloat(
     x: unc_variable,
-    default_tag: str = Number.DEFAULT,
+    default_tag: UncertaintyFlag | str = UncertaintyFlag.DEFAULT,
 ) -> tuple[float, dict[str, float | NDArray]]:
     """
     Takes a ``ufloat`` object *x* from the "uncertainties" package and returns a tuple with two
     elements containing its nominal value and a dictionary with its uncertainties. When the error
     components of *x* contain multiple uncertainties with the same name, they are combined under the
     assumption of full correlation. When an error component is not tagged, *default_tag* is used.
     """
     # store error components to be combined per tag
     components: dict[str, list[tuple[float, float] | tuple[NDArray, NDArray]]] = defaultdict(list)
     for comp, value in x.error_components().items():  # type: ignore[attr-defined]
         name = comp.tag if comp.tag is not None else default_tag
-        components[name].append((x.derivatives[comp], value))  # type: ignore[arg-type, attr-defined]
+        components[str(name)].append((x.derivatives[comp], value))  # type: ignore[arg-type, attr-defined] # noqa
 
     # combine components to uncertainties, assume full correlation
     uncertainties = {
         name: calculate_uncertainty(terms, rho=1.0)
         for name, terms in components.items()
     }
 
@@ -2565,23 +2548,23 @@
             asym = isinstance(u, tuple)
             if asym and len(u) != 2:
                 raise ValueError(f"asymmetric uncertainties must provided as 2-tuple: {u}")
 
             _us = list(u) if asym else [u]
             if not _is_numpy:
                 for _u in _us:
-                    if not try_float(_u):
+                    if try_float(_u) is None:
                         raise TypeError(f"uncertainties must be convertible to float: {_u}")
                     if _u < 0:
                         raise ValueError(f"uncertainties must be positive: {_u}")
 
             else:
                 for j, _u in enumerate(list(_us)):
                     if not is_numpy(_u):
-                        if not try_float(_u):
+                        if try_float(_u) is None:
                             raise TypeError(f"uncertainty is neither array nor float: {_u}")
                         _us[j] = _u = _u * np.ones_like(val)
                     if (_u < 0).any():
                         raise ValueError(f"uncertainties must be positive: {_u}")
                 unc[i] = tuple(_us) if asym else _us[0]  # type: ignore[index]
 
             # store in flat list of uncertainty values
@@ -2662,15 +2645,15 @@
         (unc_strs if multi else unc_strs[0]) if has_unc else None,
         ref_mag,
     )
 
 
 def format_multiplicative_uncertainty(
     num: Number,
-    unc: str | Sequence[str] = Number.DEFAULT,
+    unc: UncertaintyFlag | str | Sequence[UncertaintyFlag | str] = UncertaintyFlag.DEFAULT,
     digits: int = 3,
     asym_threshold: float = 0.2,
 ) -> str:
     """
     Creates an inline representation of an uncertainty named *unc* of a :py:class:`Number` *num* and
     returns it. The representation makes use of the mulitiplicative factors that would scale the
     nominal to the up/down varied values. Example:
@@ -2684,16 +2667,16 @@
         # -> "1.150/0.900"  # asymmetric
 
     When the uncertainty is either symmetric within a certain number of *digits* and the smallest
     effect is below *asym_threshold*, the symmetric representation is used (first example). In any
     other case, the asymmetric version us returned.
     """
     # get both multiplicative factors
-    f_u: float = num("up", unc, factor=True)  # type: ignore[assignment]
-    f_d: float = num("down", unc, factor=True)  # type: ignore[assignment]
+    f_u: float = num(UncertaintyDirection.UP, unc, factor=True)  # type: ignore[assignment]
+    f_d: float = num(UncertaintyDirection.DOWN, unc, factor=True)  # type: ignore[assignment]
 
     # if at least one absolute effect is large, consider them asymmetric,
     # if their effects are opposite and similar, consider them symmetric
     mag_u = abs(1.0 - f_u)
     mag_d = abs(1.0 - f_d)
     sym = (
         max(mag_u, mag_d) < asym_threshold and
```

### Comparing `scinum-2.1.0/scinum.egg-info/PKG-INFO` & `scinum-2.1.1/scinum.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scinum
-Version: 2.1.0
+Version: 2.1.1
 Summary: Scientific numbers with multiple uncertainties and correlation-aware, gaussian propagation and Numpy support.
 Author-email: Marcel Rieger <marcel.rieger@cern.ch>
 License: Copyright (c) 2017-2024, Marcel Rieger
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
```

