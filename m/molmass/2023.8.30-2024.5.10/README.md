# Comparing `tmp/molmass-2023.8.30.tar.gz` & `tmp/molmass-2024.5.10.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "molmass-2023.8.30.tar", last modified: Wed Aug 30 15:23:27 2023, max compression
+gzip compressed data, was "molmass-2024.5.10.tar", last modified: Fri May 10 15:16:35 2024, max compression
```

## Comparing `molmass-2023.8.30.tar` & `molmass-2024.5.10.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-08-30 15:23:27.228168 molmass-2023.8.30/
--rw-rw-rw-   0        0        0     1559 2023-08-30 15:23:22.000000 molmass-2023.8.30/LICENSE
--rw-rw-rw-   0        0        0      305 2023-08-11 03:03:18.000000 molmass-2023.8.30/MANIFEST.in
--rw-rw-rw-   0        0        0     6730 2023-08-30 15:23:27.226077 molmass-2023.8.30/PKG-INFO
--rw-rw-rw-   0        0        0     5744 2023-08-30 15:23:22.000000 molmass-2023.8.30/README.rst
-drwxrwxrwx   0        0        0        0 2023-08-30 15:23:27.215915 molmass-2023.8.30/molmass/
--rw-rw-rw-   0        0        0      206 2022-10-18 17:06:47.000000 molmass-2023.8.30/molmass/__init__.py
--rw-rw-rw-   0        0        0      132 2020-01-01 02:11:19.000000 molmass-2023.8.30/molmass/__main__.py
--rw-rw-rw-   0        0        0    81337 2023-08-30 15:18:27.000000 molmass-2023.8.30/molmass/elements.py
--rw-rw-rw-   0        0        0    44874 2023-03-08 23:01:23.000000 molmass-2023.8.30/molmass/elements_descriptions.py
--rw-rw-rw-   0        0        0    39104 2023-08-30 03:54:59.000000 molmass-2023.8.30/molmass/elements_gui.py
--rw-rw-rw-   0        0        0      355 2010-03-08 22:00:45.000000 molmass-2023.8.30/molmass/icon.png
--rw-rw-rw-   0        0        0    74500 2023-08-30 15:13:22.000000 molmass-2023.8.30/molmass/molmass.py
--rw-rw-rw-   0        0        0        0 2023-08-11 00:10:50.000000 molmass-2023.8.30/molmass/py.typed
--rw-rw-rw-   0        0        0    19552 2023-08-30 03:55:58.000000 molmass-2023.8.30/molmass/web.py
-drwxrwxrwx   0        0        0        0 2023-08-30 15:23:27.226077 molmass-2023.8.30/molmass.egg-info/
--rw-rw-rw-   0        0        0     6730 2023-08-30 15:23:26.000000 molmass-2023.8.30/molmass.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      412 2023-08-30 15:23:27.000000 molmass-2023.8.30/molmass.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-30 15:23:26.000000 molmass-2023.8.30/molmass.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      136 2023-08-30 15:23:26.000000 molmass-2023.8.30/molmass.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       41 2023-08-30 15:23:26.000000 molmass-2023.8.30/molmass.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-08-30 15:23:26.000000 molmass-2023.8.30/molmass.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-30 15:23:27.228168 molmass-2023.8.30/setup.cfg
--rw-rw-rw-   0        0        0     2714 2023-08-30 03:54:38.000000 molmass-2023.8.30/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-10 15:16:35.642995 molmass-2024.5.10/
+-rw-rw-rw-   0        0        0     1559 2024-05-10 15:16:34.000000 molmass-2024.5.10/LICENSE
+-rw-rw-rw-   0        0        0      305 2023-08-11 03:03:18.000000 molmass-2024.5.10/MANIFEST.in
+-rw-rw-rw-   0        0        0     6986 2024-05-10 15:16:35.641995 molmass-2024.5.10/PKG-INFO
+-rw-rw-rw-   0        0        0     5877 2024-05-10 15:16:34.000000 molmass-2024.5.10/README.rst
+drwxrwxrwx   0        0        0        0 2024-05-10 15:16:35.638996 molmass-2024.5.10/molmass/
+-rw-rw-rw-   0        0        0      206 2022-10-18 17:06:47.000000 molmass-2024.5.10/molmass/__init__.py
+-rw-rw-rw-   0        0        0      132 2020-01-01 02:11:19.000000 molmass-2024.5.10/molmass/__main__.py
+-rw-rw-rw-   0        0        0    81350 2024-05-10 15:02:07.000000 molmass-2024.5.10/molmass/elements.py
+-rw-rw-rw-   0        0        0    44874 2023-03-08 23:01:23.000000 molmass-2024.5.10/molmass/elements_descriptions.py
+-rw-rw-rw-   0        0        0    39129 2024-05-10 14:59:59.000000 molmass-2024.5.10/molmass/elements_gui.py
+-rw-rw-rw-   0        0        0      355 2010-03-08 22:00:45.000000 molmass-2024.5.10/molmass/icon.png
+-rw-rw-rw-   0        0        0    76646 2024-05-10 15:16:29.000000 molmass-2024.5.10/molmass/molmass.py
+-rw-rw-rw-   0        0        0        0 2023-08-11 00:10:50.000000 molmass-2024.5.10/molmass/py.typed
+-rw-rw-rw-   0        0        0    19551 2024-01-06 17:38:30.000000 molmass-2024.5.10/molmass/web.py
+drwxrwxrwx   0        0        0        0 2024-05-10 15:16:35.641995 molmass-2024.5.10/molmass.egg-info/
+-rw-rw-rw-   0        0        0     6986 2024-05-10 15:16:35.000000 molmass-2024.5.10/molmass.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      412 2024-05-10 15:16:35.000000 molmass-2024.5.10/molmass.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-10 15:16:35.000000 molmass-2024.5.10/molmass.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      136 2024-05-10 15:16:35.000000 molmass-2024.5.10/molmass.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       41 2024-05-10 15:16:35.000000 molmass-2024.5.10/molmass.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-10 15:16:35.000000 molmass-2024.5.10/molmass.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-10 15:16:35.642995 molmass-2024.5.10/setup.cfg
+-rw-rw-rw-   0        0        0     2714 2023-08-30 03:54:38.000000 molmass-2024.5.10/setup.py
```

### Comparing `molmass-2023.8.30/LICENSE` & `molmass-2024.5.10/LICENSE`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 BSD 3-Clause License
 
-Copyright (c) 1990-2023, Christoph Gohlke
+Copyright (c) 1990-2024, Christoph Gohlke
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 1. Redistributions of source code must retain the above copyright notice,
    this list of conditions and the following disclaimer.
```

### Comparing `molmass-2023.8.30/PKG-INFO` & `molmass-2024.5.10/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molmass
-Version: 2023.8.30
+Version: 2024.5.10
 Summary: Molecular mass calculations
 Home-page: https://www.cgohlke.com
 Author: Christoph Gohlke
 Author-email: cgohlke@cgohlke.com
 License: BSD
 Project-URL: Bug Tracker, https://github.com/cgohlke/molmass/issues
 Project-URL: Source Code, https://github.com/cgohlke/molmass
@@ -17,17 +17,20 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
+License-File: LICENSE
 Provides-Extra: all
+Requires-Dist: Flask; extra == "all"
+Requires-Dist: pandas; extra == "all"
 Provides-Extra: gui
-License-File: LICENSE
+Requires-Dist: wxPython>=4.0; extra == "gui"
 
 Molecular mass calculations
 ===========================
 
 Molmass is a Python library, console script, and web application to calculate
 the molecular mass (average, nominal, and isotopic pure), the elemental
 composition, and the mass distribution spectrum of a molecule given by its
@@ -37,15 +40,15 @@
 deficiency due to chemical bonding is not taken into account.
 
 The library includes a database of physicochemical and descriptive properties
 of the chemical elements.
 
 :Author: `Christoph Gohlke <https://www.cgohlke.com>`_
 :License: BSD 3-Clause
-:Version: 2023.8.30
+:Version: 2024.5.10
 :DOI: `10.5281/zenodo.7135495 <https://doi.org/10.5281/zenodo.7135495>`_
 
 Quickstart
 ----------
 
 Install the molmass package and all dependencies from the
 `Python Package Index <https://pypi.org/project/molmass/>`_::
@@ -69,22 +72,27 @@
 
 Requirements
 ------------
 
 This revision was tested with the following requirements and dependencies
 (other versions may work):
 
-- `CPython <https://www.python.org>`_ 3.9.13, 3.10.11, 3.11.5, 3.12rc
-- `Flask <https://pypi.org/project/Flask/>`_ 2.3.3 (optional)
-- `Pandas <https://pypi.org/project/pandas/>`_ 1.5.3 (optional)
+- `CPython <https://www.python.org>`_ 3.9.13, 3.10.11, 3.11.9, 3.12.3
+- `Flask <https://pypi.org/project/Flask/>`_ 3.0.3 (optional)
+- `Pandas <https://pypi.org/project/pandas/>`_ 2.2.2 (optional)
 - `wxPython <https://pypi.org/project/wxPython/>`_ 4.2.1 (optional)
 
 Revisions
 ---------
 
+2024.5.10
+
+- Add options to disable parsing groups, oligos, fractions, arithmetic (#14).
+- Add Formula.expanded property.
+
 2023.8.30
 
 - Fix linting issues.
 - Add py.typed marker.
 - Remove support for Python 3.8.
 
 2023.4.10
@@ -232,7 +240,8 @@
 >>> len(ELEMENTS)
 109
 >>> sum(e.mass for e in ELEMENTS)
 14693.181589001...
 >>> for e in ELEMENTS:
 ...     e.validate()
 ...     e = eval(repr(e))
+...
```

### Comparing `molmass-2023.8.30/README.rst` & `molmass-2024.5.10/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 deficiency due to chemical bonding is not taken into account.
 
 The library includes a database of physicochemical and descriptive properties
 of the chemical elements.
 
 :Author: `Christoph Gohlke <https://www.cgohlke.com>`_
 :License: BSD 3-Clause
-:Version: 2023.8.30
+:Version: 2024.5.10
 :DOI: `10.5281/zenodo.7135495 <https://doi.org/10.5281/zenodo.7135495>`_
 
 Quickstart
 ----------
 
 Install the molmass package and all dependencies from the
 `Python Package Index <https://pypi.org/project/molmass/>`_::
@@ -42,22 +42,27 @@
 
 Requirements
 ------------
 
 This revision was tested with the following requirements and dependencies
 (other versions may work):
 
-- `CPython <https://www.python.org>`_ 3.9.13, 3.10.11, 3.11.5, 3.12rc
-- `Flask <https://pypi.org/project/Flask/>`_ 2.3.3 (optional)
-- `Pandas <https://pypi.org/project/pandas/>`_ 1.5.3 (optional)
+- `CPython <https://www.python.org>`_ 3.9.13, 3.10.11, 3.11.9, 3.12.3
+- `Flask <https://pypi.org/project/Flask/>`_ 3.0.3 (optional)
+- `Pandas <https://pypi.org/project/pandas/>`_ 2.2.2 (optional)
 - `wxPython <https://pypi.org/project/wxPython/>`_ 4.2.1 (optional)
 
 Revisions
 ---------
 
+2024.5.10
+
+- Add options to disable parsing groups, oligos, fractions, arithmetic (#14).
+- Add Formula.expanded property.
+
 2023.8.30
 
 - Fix linting issues.
 - Add py.typed marker.
 - Remove support for Python 3.8.
 
 2023.4.10
@@ -205,7 +210,8 @@
 >>> len(ELEMENTS)
 109
 >>> sum(e.mass for e in ELEMENTS)
 14693.181589001...
 >>> for e in ELEMENTS:
 ...     e.validate()
 ...     e = eval(repr(e))
+...
```

### Comparing `molmass-2023.8.30/molmass/elements.py` & `molmass-2024.5.10/molmass/elements.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # molmass/elements.py
 
-# Copyright (c) 2005-2023, Christoph Gohlke
+# Copyright (c) 2005-2024, Christoph Gohlke
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #
 # 1. Redistributions of source code must retain the above copyright notice,
 #    this list of conditions and the following disclaimer.
@@ -41,15 +41,15 @@
    atomic-weights-and-isotopic-compositions-relative-atomic-masses
 2. https://en.wikipedia.org/wiki/{element.name}
 
 """
 
 from __future__ import annotations
 
-__version__ = '2023.8.30'
+__version__ = '2024.5.10'
 
 __all__ = [
     'Element',
     'Isotope',
     'Particle',
     'ELECTRON',
     'ELEMENTARY_CHARGE',
@@ -2119,14 +2119,15 @@
     Examples:
         >>> import sqlite3
         >>> con = sqlite3.connect(':memory:')
         >>> cur = con.executescript(sqlite_script())
         >>> con.commit()
         >>> for r in cur.execute("SELECT name FROM element WHERE number=6"):
         ...     str(r[0])
+        ...
         'Carbon'
         >>> con.close()
 
     """
     sql = [
         """
         CREATE TABLE "period" (
```

### Comparing `molmass-2023.8.30/molmass/elements_descriptions.py` & `molmass-2024.5.10/molmass/elements_descriptions.py`

 * *Files identical despite different names*

### Comparing `molmass-2023.8.30/molmass/elements_gui.py` & `molmass-2024.5.10/molmass/elements_gui.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # elements_gui.py
 
-# Copyright (c) 2005-2022, Christoph Gohlke
+# Copyright (c) 2005-2024, Christoph Gohlke
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #
 # 1. Redistributions of source code must retain the above copyright notice,
 #    this list of conditions and the following disclaimer.
@@ -44,24 +44,24 @@
 import os
 import sys
 
 import wx
 from wx.lib import buttons, fancytext, rcsizer
 
 try:
-    from .elements import ELEMENTS, SERIES
+    from .elements import ELEMENTS, SERIES, __version__
 except ImportError:
-    from elements import ELEMENTS, SERIES  # type: ignore
+    from elements import ELEMENTS, SERIES, __version__  # type: ignore
 
 
 class MainApp(wx.App):
     """Main application."""
 
     name = 'Periodic Table of Elements'
-    version = '2022.10.18'
+    version = __version__
     website = 'https://www.cgohlke.com'
     copyright = 'Christoph Gohlke'
     icon = 'icon.png'
     try:
         icon = os.path.join(os.path.dirname(__file__), icon)
     except Exception:
         pass
```

### Comparing `molmass-2023.8.30/molmass/molmass.py` & `molmass-2024.5.10/molmass/molmass.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # molmass.py
 
-# Copyright (c) 1990-2023, Christoph Gohlke
+# Copyright (c) 1990-2024, Christoph Gohlke
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #
 # 1. Redistributions of source code must retain the above copyright notice,
 #    this list of conditions and the following disclaimer.
@@ -40,15 +40,15 @@
 deficiency due to chemical bonding is not taken into account.
 
 The library includes a database of physicochemical and descriptive properties
 of the chemical elements.
 
 :Author: `Christoph Gohlke <https://www.cgohlke.com>`_
 :License: BSD 3-Clause
-:Version: 2023.8.30
+:Version: 2024.5.10
 :DOI: `10.5281/zenodo.7135495 <https://doi.org/10.5281/zenodo.7135495>`_
 
 Quickstart
 ----------
 
 Install the molmass package and all dependencies from the
 `Python Package Index <https://pypi.org/project/molmass/>`_::
@@ -72,22 +72,27 @@
 
 Requirements
 ------------
 
 This revision was tested with the following requirements and dependencies
 (other versions may work):
 
-- `CPython <https://www.python.org>`_ 3.9.13, 3.10.11, 3.11.5, 3.12rc
-- `Flask <https://pypi.org/project/Flask/>`_ 2.3.3 (optional)
-- `Pandas <https://pypi.org/project/pandas/>`_ 1.5.3 (optional)
+- `CPython <https://www.python.org>`_ 3.9.13, 3.10.11, 3.11.9, 3.12.3
+- `Flask <https://pypi.org/project/Flask/>`_ 3.0.3 (optional)
+- `Pandas <https://pypi.org/project/pandas/>`_ 2.2.2 (optional)
 - `wxPython <https://pypi.org/project/wxPython/>`_ 4.2.1 (optional)
 
 Revisions
 ---------
 
+2024.5.10
+
+- Add options to disable parsing groups, oligos, fractions, arithmetic (#14).
+- Add Formula.expanded property.
+
 2023.8.30
 
 - Fix linting issues.
 - Add py.typed marker.
 - Remove support for Python 3.8.
 
 2023.4.10
@@ -235,20 +240,21 @@
 >>> len(ELEMENTS)
 109
 >>> sum(e.mass for e in ELEMENTS)
 14693.181589001...
 >>> for e in ELEMENTS:
 ...     e.validate()
 ...     e = eval(repr(e))
+...
 
 """
 
 from __future__ import annotations
 
-__version__ = '2023.8.30'
+__version__ = '2024.5.10'
 
 __all__ = [
     'Composition',
     'CompositionItem',
     'Formula',
     'FormulaError',
     'Spectrum',
@@ -278,16 +284,15 @@
 import re
 import sys
 from dataclasses import dataclass
 from functools import cached_property, reduce
 from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
-    from collections.abc import Iterable, Iterator, Sequence
-    from typing import Callable
+    from collections.abc import Callable, Iterable, Iterator, Sequence
 
     import pandas
 
 try:
     from .elements import ELECTRON, ELEMENTS, Isotope
 except ImportError:
     from elements import ELECTRON, ELEMENTS, Isotope  # type: ignore
@@ -397,14 +402,22 @@
             Chemical formula. May contain only symbols of chemical elements,
             groups, isotopes, parentheses, numbers, and trailing charge.
             The formula is not validated until it is parsed on demand
             during instance attribute access or method calls.
         groups:
             Mapping of chemical group name to formula in Hill notation.
             The default is :py:attr:`GROUPS`.
+        parse_groups:
+            Parse chemical group names. Enabled by default.
+        parse_oligos:
+            Parse pure peptide and nucleotide sequences. Enabled by default.
+        parse_fractions:
+            Parse list of mass fractions. Enabled by default.
+        parse_arithmetic:
+            Parse simple arithmetic operators. Enabled by default.
 
     Examples:
         Elements and counts:
 
         >>> Formula('H2O')
         Formula('H2O')
 
@@ -463,18 +476,30 @@
     _charge: int
     _formula: str
     _formula_nocharge: str
 
     def __init__(
         self,
         formula: str = '',
-        groups: dict[str, str] | None = None,
         /,
+        groups: dict[str, str] | None = None,
+        *,
+        parse_groups: bool = True,
+        parse_oligos: bool = True,
+        parse_fractions: bool = True,
+        parse_arithmetic: bool = True,
     ) -> None:
-        self._formula = from_string(formula, groups)
+        self._formula = from_string(
+            formula,
+            groups,
+            parse_groups,
+            parse_oligos,
+            parse_fractions,
+            parse_arithmetic,
+        )
         self._formula_nocharge, self._charge = split_charge(self._formula)
 
     @cached_property
     def _elements(self) -> dict[str, dict[int, int]]:
         """Number of atoms and isotopes by element.
 
         A ``dict[symbol: dict[massnumber: count]]``, where `massnumber` is
@@ -618,14 +643,26 @@
         '[O4S]2-'
 
         """
         return from_elements(
             self._elements, charge=self._charge, divisor=self.gcd
         )
 
+    @property
+    def expanded(self) -> str:
+        """Formula string with expanded groups, charges, and sequences.
+
+        The input formula parsed by :py:func:`from_string`.
+
+        >>> Formula('WQ').expanded  # peptide sequence
+        '((C5H8N2O2)(C11H10N2O)H2O)'
+
+        """
+        return self._formula
+
     @cached_property
     def atoms(self) -> int:
         """Number of atoms.
 
         >>> Formula('CH3COOH').atoms
         8
 
@@ -1384,85 +1421,109 @@
 
     def __str__(self) -> str:
         if self.position < 0:
             return str(self.message)
         return f"{self.message}\n{self.formula}\n{'.' * self.position}^"
 
 
-def from_string(formula: str, groups: dict[str, str] | None = None, /) -> str:
+def from_string(
+    formula: str,
+    /,
+    groups: dict[str, str] | None = None,
+    parse_groups: bool = True,
+    parse_oligos: bool = True,
+    parse_fractions: bool = True,
+    parse_arithmetic: bool = True,
+) -> str:
     r"""Return formula string from user input string.
 
     Parameters:
         formula:
             Chemical formula.
             Supports simple, non-nested arithmetic (\+ and \*), abbreviations
             of common chemical groups, peptides, oligos, and mass fractions.
         groups:
             Mapping of chemical group name to formula in Hill notation.
             The default is :py:attr:`GROUPS`.
+        parse_groups:
+            Parse chemical group names.
+        parse_oligos:
+            Parse pure peptide and nucleotide sequences.
+        parse_fractions:
+            Parse list of mass fractions.
+        parse_arithmetic:
+            Parse simple arithmetic operators.
 
     Returns:
         Chemical formula composed only of element and isotope symbols,
         parentheses, numbers, and trailing ion charges.
 
     Raises:
         FormulaError: Invalid formula.
 
     Examples:
         >>> from_string('Valohp')
         '(C5H8NO2)'
+        >>> from_string('Valohp', parse_groups=False)
+        'Valohp'
         >>> from_string('HLeu2OH')
         'H(C6H11NO)2OH'
         >>> from_string('D2O')
         '[2H]2O'
         >>> from_string('O: 0.26, 30Si: 0.74')
         'O2[30Si]3'
+        >>> from_string('O: 0.26, 30Si: 0.74', parse_fractions=False)
+        'O:0(,30Si:0)26()74'
         >>> from_string('PhNH2.HCl')
         '(C6H5)NH2HCl'
+        >>> from_string('PhNH2.HCl', parse_arithmetic=False)
+        '(C6H5)NH2.HCl'
         >>> from_string('CuSO4.5H2O')
         'CuSO4(H2O)5'
         >>> from_string('CuSO4+5*H2O')
         'CuSO4(H2O)5'
         >>> from_string('5*H2O')
         '(H2O)5'
         >>> from_string('O2+12C')  # not [12C]O2
         'O2(C)12'
         >>> from_string('ssdna(AC)')
         '((C10H12N5O5P)(C9H12N3O6P)H2O)'
         >>> from_string('peptide(GG)')
         '((C2H3NO)2H2O)'
+        >>> from_string('WQ')
+        '((C5H8N2O2)(C11H10N2O)H2O)'
+        >>> from_string('WQ', parse_oligos=False)
+        'WQ'
 
     """
     try:
         formula = formula.strip().replace(' ', '')
     except AttributeError as exc:
         raise ValueError('formula must be a string') from exc
 
-    # abbreviations of common chemical groups
-    if groups is None:
-        groups = GROUPS
-    if groups:
-        for grp in reversed(sorted(groups)):
-            formula = formula.replace(grp, f'({groups[grp]})')
+    if parse_groups:
+        if groups is None:
+            groups = GROUPS
+        if groups:
+            for grp in reversed(sorted(groups)):
+                formula = formula.replace(grp, f'({groups[grp]})')
 
-    # list of mass fractions
-    if ':' in formula and ',' in formula:
+    if parse_fractions and ':' in formula and ',' in formula:
         fractions: dict[str, float] = {}
         try:
             for item in formula.split(','):
                 items = item.split(':')
                 fractions[items[0].strip()] = float(items[1].strip())
         except Exception as exc:
             raise FormulaError(
                 'invalid list of mass fractions', formula
             ) from exc
         return from_fractions(fractions)
 
-    # oligos and peptides
-    if len(formula) > 1:
+    if parse_oligos and len(formula) > 1:
         fset = set(formula)
         if fset <= set('ATCG') and fset & set('ATG'):
             return from_oligo(formula, 'ssdna')
         if fset <= set('AUCG') and fset & set('AG'):
             return from_oligo(formula, 'ssrna')
         if fset <= set(AMINOACIDS.keys()) and fset & set('AEGMLQRT'):
             return from_peptide(formula)
@@ -1472,32 +1533,32 @@
 
     # Deuterium
     formula = re.sub('(D)(?![a-z])', '[2H]', formula)
 
     # charge
     formula, charge = split_charge(formula)
 
-    # arithmetic
-    formula = formula.replace('.', '+')
-    if '+' in formula or '*' in formula:
-        # TODO: document O2+12C is C12O2, not [12C]O2
-        for match in re.findall(
-            r'(?:\+|^)((\d+)\*?(.*?))(?:(?=\+)|$)', formula
-        ):
-            formula = formula.replace(match[0], f'({match[2]}){match[1]}')
-        m = re.search(r'(\+[a-z])', formula)
-        if m:
+    if parse_arithmetic:
+        formula = formula.replace('.', '+')
+        if '+' in formula or '*' in formula:
+            # TODO: document O2+12C is C12O2, not [12C]O2
+            for match in re.findall(
+                r'(?:\+|^)((\d+)\*?(.*?))(?:(?=\+)|$)', formula
+            ):
+                formula = formula.replace(match[0], f'({match[2]}){match[1]}')
+            m = re.search(r'(\+[a-z])', formula)
+            if m:
+                raise FormulaError(
+                    'invalid symbol', formula, formula.index(m[0]) + 1
+                )
+            formula = formula.replace('+', '')
+        if '-' in formula:
             raise FormulaError(
-                'invalid symbol', formula, formula.index(m[0]) + 1
+                'subtraction not allowed', formula, formula.index('-')
             )
-        formula = formula.replace('+', '')
-    if '-' in formula:
-        raise FormulaError(
-            'subtraction not allowed', formula, formula.index('-')
-        )
 
     if charge != 0:
         formula = f'[{formula}]{format_charge(charge)}'
     return formula
 
 
 def from_elements(
@@ -1522,16 +1583,23 @@
             Format strings.
 
     Examples:
         >>> from_elements({'C': {0: 4, 12: 2}}, divisor=2)
         'C2[12C]'
 
         >>> from_elements(
-        ...     {'C': {0: 4, 12: 2}}, divisor=2, fmt=('{}', '{}<sub>{}</sub>',
-        ...     '<sup>{}</sup>{}', '<sup>{}</sup>{}<sub>{}</sub>'))
+        ...     {'C': {0: 4, 12: 2}},
+        ...     divisor=2,
+        ...     fmt=(
+        ...         '{}',
+        ...         '{}<sub>{}</sub>',
+        ...         '<sup>{}</sup>{}',
+        ...         '<sup>{}</sup>{}<sub>{}</sub>',
+        ...     ),
+        ... )
         'C<sub>2</sub><sup>12</sup>C'
 
     """
     if fmt is None:
         fmt = ('{}', '{}{}', '[{}{}]', '[{}{}]{}')
     formula = []
     for symbol in hill_sorted(elements):
```

### Comparing `molmass-2023.8.30/molmass/web.py` & `molmass-2024.5.10/molmass/web.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python3
 # molmass/web.py
 
-# Copyright (c) 2005-2023, Christoph Gohlke
+# Copyright (c) 2005-2024, Christoph Gohlke
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #
 # 1. Redistributions of source code must retain the above copyright notice,
 #    this list of conditions and the following disclaimer.
@@ -353,15 +353,15 @@
             if abs(spectrum._charge) > 1:
                 mz = '\n<th scope="col">m/z</th>'
             else:
                 mz = ''
             result.extend(
                 (
                     '<!--h3>Mass Distribution</h3-->',
-                    '<table class="table">'
+                    '<table class="table">',
                     '<caption>Mass Distribution</caption>',
                     '<tr>',
                     '<th scope="col">Mass number</th>',
                     '<th scope="col">Relative mass</th>',
                     '<th scope="col">Fraction %</th>',
                     '<th scope="col">Intensity %</th>',
                     mz,
@@ -393,15 +393,14 @@
         )
 
     return '\n'.join(i for i in result if i)
 
 
 def isotopes() -> str:
     """Return HTML table of isotope masses and abundances."""
-
     template = """
     <!--h2>Isotopic Composition of the Elements</h2-->
     <table>
     <caption>Isotopic Composition of the Elements</caption>
     <tr>
     <th scope="col">Element/Isotope</th>
     <th scope="col" align="right">Relative mass</th>
@@ -434,15 +433,14 @@
                 )
             )
     return template.format(rows='\n'.join(rows))
 
 
 def groups() -> str:
     """Return HTML table of chemical groups."""
-
     template = """
     <!--h3>{title}</h3-->
     <table>
     <caption>{title}</caption>
     <tr>
     <th scope="col">Name</th>
     <th scope="col">Formula</th>
```

### Comparing `molmass-2023.8.30/molmass.egg-info/PKG-INFO` & `molmass-2024.5.10/molmass.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molmass
-Version: 2023.8.30
+Version: 2024.5.10
 Summary: Molecular mass calculations
 Home-page: https://www.cgohlke.com
 Author: Christoph Gohlke
 Author-email: cgohlke@cgohlke.com
 License: BSD
 Project-URL: Bug Tracker, https://github.com/cgohlke/molmass/issues
 Project-URL: Source Code, https://github.com/cgohlke/molmass
@@ -17,17 +17,20 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
+License-File: LICENSE
 Provides-Extra: all
+Requires-Dist: Flask; extra == "all"
+Requires-Dist: pandas; extra == "all"
 Provides-Extra: gui
-License-File: LICENSE
+Requires-Dist: wxPython>=4.0; extra == "gui"
 
 Molecular mass calculations
 ===========================
 
 Molmass is a Python library, console script, and web application to calculate
 the molecular mass (average, nominal, and isotopic pure), the elemental
 composition, and the mass distribution spectrum of a molecule given by its
@@ -37,15 +40,15 @@
 deficiency due to chemical bonding is not taken into account.
 
 The library includes a database of physicochemical and descriptive properties
 of the chemical elements.
 
 :Author: `Christoph Gohlke <https://www.cgohlke.com>`_
 :License: BSD 3-Clause
-:Version: 2023.8.30
+:Version: 2024.5.10
 :DOI: `10.5281/zenodo.7135495 <https://doi.org/10.5281/zenodo.7135495>`_
 
 Quickstart
 ----------
 
 Install the molmass package and all dependencies from the
 `Python Package Index <https://pypi.org/project/molmass/>`_::
@@ -69,22 +72,27 @@
 
 Requirements
 ------------
 
 This revision was tested with the following requirements and dependencies
 (other versions may work):
 
-- `CPython <https://www.python.org>`_ 3.9.13, 3.10.11, 3.11.5, 3.12rc
-- `Flask <https://pypi.org/project/Flask/>`_ 2.3.3 (optional)
-- `Pandas <https://pypi.org/project/pandas/>`_ 1.5.3 (optional)
+- `CPython <https://www.python.org>`_ 3.9.13, 3.10.11, 3.11.9, 3.12.3
+- `Flask <https://pypi.org/project/Flask/>`_ 3.0.3 (optional)
+- `Pandas <https://pypi.org/project/pandas/>`_ 2.2.2 (optional)
 - `wxPython <https://pypi.org/project/wxPython/>`_ 4.2.1 (optional)
 
 Revisions
 ---------
 
+2024.5.10
+
+- Add options to disable parsing groups, oligos, fractions, arithmetic (#14).
+- Add Formula.expanded property.
+
 2023.8.30
 
 - Fix linting issues.
 - Add py.typed marker.
 - Remove support for Python 3.8.
 
 2023.4.10
@@ -232,7 +240,8 @@
 >>> len(ELEMENTS)
 109
 >>> sum(e.mass for e in ELEMENTS)
 14693.181589001...
 >>> for e in ELEMENTS:
 ...     e.validate()
 ...     e = eval(repr(e))
+...
```

### Comparing `molmass-2023.8.30/setup.py` & `molmass-2024.5.10/setup.py`

 * *Files identical despite different names*

