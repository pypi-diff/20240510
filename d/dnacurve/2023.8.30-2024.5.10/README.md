# Comparing `tmp/dnacurve-2023.8.30.tar.gz` & `tmp/dnacurve-2024.5.10.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dnacurve-2023.8.30.tar", last modified: Wed Aug 30 07:45:33 2023, max compression
+gzip compressed data, was "dnacurve-2024.5.10.tar", last modified: Fri May 10 15:42:10 2024, max compression
```

## Comparing `dnacurve-2023.8.30.tar` & `dnacurve-2024.5.10.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-08-30 07:45:33.145609 dnacurve-2023.8.30/
--rw-rw-rw-   0        0        0     1559 2023-08-30 07:45:28.000000 dnacurve-2023.8.30/LICENSE
--rw-rw-rw-   0        0        0      280 2023-08-11 03:05:17.000000 dnacurve-2023.8.30/MANIFEST.in
--rw-rw-rw-   0        0        0     5419 2023-08-30 07:45:33.145609 dnacurve-2023.8.30/PKG-INFO
--rw-rw-rw-   0        0        0     4456 2023-08-30 07:45:28.000000 dnacurve-2023.8.30/README.rst
-drwxrwxrwx   0        0        0        0 2023-08-30 07:45:33.145609 dnacurve-2023.8.30/dnacurve/
--rw-rw-rw-   0        0        0      104 2022-10-03 02:34:01.000000 dnacurve-2023.8.30/dnacurve/__init__.py
--rw-rw-rw-   0        0        0      135 2020-01-01 02:14:51.000000 dnacurve-2023.8.30/dnacurve/__main__.py
--rw-rw-rw-   0        0        0    55502 2023-08-30 05:54:47.000000 dnacurve-2023.8.30/dnacurve/dnacurve.py
--rw-rw-rw-   0        0        0        0 2023-08-11 00:10:50.000000 dnacurve-2023.8.30/dnacurve/py.typed
--rw-rw-rw-   0        0        0    15961 2023-08-30 04:48:28.000000 dnacurve-2023.8.30/dnacurve/web.py
-drwxrwxrwx   0        0        0        0 2023-08-30 07:45:33.145609 dnacurve-2023.8.30/dnacurve.egg-info/
--rw-rw-rw-   0        0        0     5419 2023-08-30 07:45:32.000000 dnacurve-2023.8.30/dnacurve.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      330 2023-08-30 07:45:32.000000 dnacurve-2023.8.30/dnacurve.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-30 07:45:32.000000 dnacurve-2023.8.30/dnacurve.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       85 2023-08-30 07:45:32.000000 dnacurve-2023.8.30/dnacurve.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       30 2023-08-30 07:45:32.000000 dnacurve-2023.8.30/dnacurve.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-08-30 07:45:32.000000 dnacurve-2023.8.30/dnacurve.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-30 07:45:33.145609 dnacurve-2023.8.30/setup.cfg
--rw-rw-rw-   0        0        0     2630 2023-08-30 04:48:13.000000 dnacurve-2023.8.30/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-10 15:42:10.352996 dnacurve-2024.5.10/
+-rw-rw-rw-   0        0        0     1559 2024-05-10 15:42:09.000000 dnacurve-2024.5.10/LICENSE
+-rw-rw-rw-   0        0        0      280 2023-08-11 03:05:17.000000 dnacurve-2024.5.10/MANIFEST.in
+-rw-rw-rw-   0        0        0     5541 2024-05-10 15:42:10.352996 dnacurve-2024.5.10/PKG-INFO
+-rw-rw-rw-   0        0        0     4491 2024-05-10 15:42:09.000000 dnacurve-2024.5.10/README.rst
+drwxrwxrwx   0        0        0        0 2024-05-10 15:42:10.349996 dnacurve-2024.5.10/dnacurve/
+-rw-rw-rw-   0        0        0      104 2022-10-03 02:34:01.000000 dnacurve-2024.5.10/dnacurve/__init__.py
+-rw-rw-rw-   0        0        0      135 2020-01-01 02:14:51.000000 dnacurve-2024.5.10/dnacurve/__main__.py
+-rw-rw-rw-   0        0        0    55514 2024-05-10 15:41:51.000000 dnacurve-2024.5.10/dnacurve/dnacurve.py
+-rw-rw-rw-   0        0        0        0 2023-08-11 00:10:50.000000 dnacurve-2024.5.10/dnacurve/py.typed
+-rw-rw-rw-   0        0        0    15961 2023-12-25 05:05:11.000000 dnacurve-2024.5.10/dnacurve/web.py
+drwxrwxrwx   0        0        0        0 2024-05-10 15:42:10.351996 dnacurve-2024.5.10/dnacurve.egg-info/
+-rw-rw-rw-   0        0        0     5541 2024-05-10 15:42:10.000000 dnacurve-2024.5.10/dnacurve.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      330 2024-05-10 15:42:10.000000 dnacurve-2024.5.10/dnacurve.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-10 15:42:10.000000 dnacurve-2024.5.10/dnacurve.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       85 2024-05-10 15:42:10.000000 dnacurve-2024.5.10/dnacurve.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       30 2024-05-10 15:42:10.000000 dnacurve-2024.5.10/dnacurve.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-10 15:42:10.000000 dnacurve-2024.5.10/dnacurve.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-10 15:42:10.352996 dnacurve-2024.5.10/setup.cfg
+-rw-rw-rw-   0        0        0     2630 2023-08-30 04:48:13.000000 dnacurve-2024.5.10/setup.py
```

### Comparing `dnacurve-2023.8.30/LICENSE` & `dnacurve-2024.5.10/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 BSD 3-Clause License
 
-Copyright (c) 1993-2023, Christoph Gohlke
+Copyright (c) 1993-2024, Christoph Gohlke
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 1. Redistributions of source code must retain the above copyright notice,
    this list of conditions and the following disclaimer.
```

### Comparing `dnacurve-2023.8.30/PKG-INFO` & `dnacurve-2024.5.10/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dnacurve
-Version: 2023.8.30
+Version: 2024.5.10
 Summary: DNA curvature analysis
 Home-page: https://www.cgohlke.com
 Author: Christoph Gohlke
 Author-email: cgohlke@cgohlke.com
 License: BSD
 Project-URL: Bug Tracker, https://github.com/cgohlke/dnacurve/issues
 Project-URL: Source Code, https://github.com/cgohlke/dnacurve
@@ -17,28 +17,31 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
-Provides-Extra: all
 License-File: LICENSE
+Requires-Dist: numpy
+Requires-Dist: matplotlib
+Provides-Extra: all
+Requires-Dist: Flask; extra == "all"
 
 DNA curvature analysis
 ======================
 
 Dnacurve is a Python library, console script, and web application to calculate
 the global 3D structure of a B-DNA molecule from its nucleotide sequence
 according to the dinucleotide wedge model. Local bending angles and macroscopic
 curvature are calculated at each nucleotide.
 
 :Author: `Christoph Gohlke <https://www.cgohlke.com>`_
 :License: BSD 3-Clause
-:Version: 2023.8.30
+:Version: 2024.5.10
 :DOI: `10.5281/zenodo.7135499 <https://doi.org/10.5281/zenodo.7135499>`_
 
 Quickstart
 ----------
 
 Install the dnacurve package and all dependencies from the
 `Python Package Index <https://pypi.org/project/dnacurve/>`_::
@@ -60,22 +63,26 @@
 
 Requirements
 ------------
 
 This revision was tested with the following requirements and dependencies
 (other versions may work):
 
-- `CPython <https://www.python.org>`_ 3.9.13, 3.10.11, 3.11.5, 3.12rc
-- `Numpy <https://pypi.org/project/numpy/>`_ 1.25.2
-- `Matplotlib <https://pypi.org/project/matplotlib/>`_ 3.7.2
-- `Flask <https://pypi.org/project/Flask/>`_ 2.3.3 (optional)
+- `CPython <https://www.python.org>`_ 3.9.13, 3.10.11, 3.11.9, 3.12.3
+- `Numpy <https://pypi.org/project/numpy/>`_ 1.26.4
+- `Matplotlib <https://pypi.org/project/matplotlib/>`_ 3.8.4
+- `Flask <https://pypi.org/project/Flask/>`_ 3.0.3 (optional)
 
 Revisions
 ---------
 
+2024.5.10
+
+- Fix mypy errors.
+
 2023.8.30
 
 - Fix linting issues.
 - Add py.typed marker.
 
 2023.4.30
```

### Comparing `dnacurve-2023.8.30/README.rst` & `dnacurve-2024.5.10/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 Dnacurve is a Python library, console script, and web application to calculate
 the global 3D structure of a B-DNA molecule from its nucleotide sequence
 according to the dinucleotide wedge model. Local bending angles and macroscopic
 curvature are calculated at each nucleotide.
 
 :Author: `Christoph Gohlke <https://www.cgohlke.com>`_
 :License: BSD 3-Clause
-:Version: 2023.8.30
+:Version: 2024.5.10
 :DOI: `10.5281/zenodo.7135499 <https://doi.org/10.5281/zenodo.7135499>`_
 
 Quickstart
 ----------
 
 Install the dnacurve package and all dependencies from the
 `Python Package Index <https://pypi.org/project/dnacurve/>`_::
@@ -34,22 +34,26 @@
 
 Requirements
 ------------
 
 This revision was tested with the following requirements and dependencies
 (other versions may work):
 
-- `CPython <https://www.python.org>`_ 3.9.13, 3.10.11, 3.11.5, 3.12rc
-- `Numpy <https://pypi.org/project/numpy/>`_ 1.25.2
-- `Matplotlib <https://pypi.org/project/matplotlib/>`_ 3.7.2
-- `Flask <https://pypi.org/project/Flask/>`_ 2.3.3 (optional)
+- `CPython <https://www.python.org>`_ 3.9.13, 3.10.11, 3.11.9, 3.12.3
+- `Numpy <https://pypi.org/project/numpy/>`_ 1.26.4
+- `Matplotlib <https://pypi.org/project/matplotlib/>`_ 3.8.4
+- `Flask <https://pypi.org/project/Flask/>`_ 3.0.3 (optional)
 
 Revisions
 ---------
 
+2024.5.10
+
+- Fix mypy errors.
+
 2023.8.30
 
 - Fix linting issues.
 - Add py.typed marker.
 
 2023.4.30
```

### Comparing `dnacurve-2023.8.30/dnacurve/dnacurve.py` & `dnacurve-2024.5.10/dnacurve/dnacurve.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # dnacurve.py
 
-# Copyright (c) 1993-2023, Christoph Gohlke
+# Copyright (c) 1993-2024, Christoph Gohlke
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #
 # 1. Redistributions of source code must retain the above copyright notice,
 #    this list of conditions and the following disclaimer.
@@ -34,15 +34,15 @@
 Dnacurve is a Python library, console script, and web application to calculate
 the global 3D structure of a B-DNA molecule from its nucleotide sequence
 according to the dinucleotide wedge model. Local bending angles and macroscopic
 curvature are calculated at each nucleotide.
 
 :Author: `Christoph Gohlke <https://www.cgohlke.com>`_
 :License: BSD 3-Clause
-:Version: 2023.8.30
+:Version: 2024.5.10
 :DOI: `10.5281/zenodo.7135499 <https://doi.org/10.5281/zenodo.7135499>`_
 
 Quickstart
 ----------
 
 Install the dnacurve package and all dependencies from the
 `Python Package Index <https://pypi.org/project/dnacurve/>`_::
@@ -64,22 +64,26 @@
 
 Requirements
 ------------
 
 This revision was tested with the following requirements and dependencies
 (other versions may work):
 
-- `CPython <https://www.python.org>`_ 3.9.13, 3.10.11, 3.11.5, 3.12rc
-- `Numpy <https://pypi.org/project/numpy/>`_ 1.25.2
-- `Matplotlib <https://pypi.org/project/matplotlib/>`_ 3.7.2
-- `Flask <https://pypi.org/project/Flask/>`_ 2.3.3 (optional)
+- `CPython <https://www.python.org>`_ 3.9.13, 3.10.11, 3.11.9, 3.12.3
+- `Numpy <https://pypi.org/project/numpy/>`_ 1.26.4
+- `Matplotlib <https://pypi.org/project/matplotlib/>`_ 3.8.4
+- `Flask <https://pypi.org/project/Flask/>`_ 3.0.3 (optional)
 
 Revisions
 ---------
 
+2024.5.10
+
+- Fix mypy errors.
+
 2023.8.30
 
 - Fix linting issues.
 - Add py.typed marker.
 
 2023.4.30
 
@@ -193,15 +197,15 @@
 >>> result.write_pdb('_test.pdb')
 >>> result.plot('_test.png', dpi=120)
 
 """
 
 from __future__ import annotations
 
-__version__ = '2023.8.30'
+__version__ = '2024.5.10'
 
 __all__ = [
     'CurvedDNA',
     'Model',
     'Sequence',
     'MAXLEN',
     'MODELS',
@@ -633,18 +637,17 @@
             return None
 
         if arg is True:
             # GUI plot
             from matplotlib import pyplot
 
             fig = pyplot.figure(dpi=dpi, figsize=figsize)
-            try:
-                fig.canvas.manager.window.title('DNA Curvature Analysis')
-            except AttributeError:
-                pass
+            fcm = fig.canvas.manager
+            if fcm is not None:
+                fcm.set_window_title('DNA Curvature Analysis')
         else:
             from matplotlib.backends.backend_agg import FigureCanvasAgg
             from matplotlib.figure import Figure
 
             fig = Figure(dpi=dpi, figsize=figsize)
             FigureCanvasAgg(fig)
 
@@ -706,15 +709,15 @@
                     xyz[1, -1, ax1],
                     "3'",
                     color='darkred',
                     clip_on=True,
                     size=10,
                 )
             ax.axis('image')
-            ax.axis([-limit, limit, -limit, limit])
+            ax.axis((-limit, limit, -limit, limit))
             ax.axis('off')
 
         plot_projection(322, 'XZ')
         plot_projection(323, 'ZY', False)
         plot_projection(324, 'XY')
 
         # plot
@@ -807,17 +810,17 @@
         >>> m = Model(Model.CALLADINE, name='My Model', rise=4.0)
         >>> m.name == 'My Model' and m.rise == 4.0
         True
         >>> m = Model(
         ...     name='Test',
         ...     rise=3.38,
         ...     oligo='AA AC AG AT CA GG CG GA GC TA'.split(),
-        ...     twist=(34.29, ) * 10,
-        ...     roll=(0., ) * 10,
-        ...     tilt=(0., ) * 10,
+        ...     twist=(34.29,) * 10,
+        ...     roll=(0.0,) * 10,
+        ...     tilt=(0.0,) * 10,
         ... )
         >>> m.write('_test.dat')
         >>> m.twist == Model('_test.dat').twist
         True
 
     """
 
@@ -1312,36 +1315,34 @@
             s.remove(oligo)
         else:
             s.add(complementary(oligo))
             yield oligo
 
 
 @overload
-def chunks(sequence: str, size: int = 10, /) -> list[str]:
-    ...
+def chunks(sequence: str, size: int = 10, /) -> list[str]: ...
 
 
 @overload
-def chunks(sequence: list[str], size: int = 10, /) -> list[list[str]]:
-    ...
+def chunks(sequence: list[str], size: int = 10, /) -> list[list[str]]: ...
 
 
 def chunks(
     sequence: str | list[str],
     /,
     size: int = 10,
 ) -> list[str] | list[list[str]]:
     """Return sequence in chunks of size.
 
     Parameters:
         sequence: Sequence to be chunked.
         size: Length of chunks.
 
     Examples:
-        >>> chunks('ATCG'*4, 10)
+        >>> chunks('ATCG' * 4, 10)
         ['ATCGATCGAT', 'CGATCG']
 
     """
     return [  # type: ignore
         sequence[i : i + size] for i in range(0, len(sequence), size)
     ]
 
@@ -1356,15 +1357,15 @@
         size: Length of chunks.
         overlap: Size of overlap.
 
     Yields:
         Tuple of start position of chunk and chunk sequence.
 
     Examples:
-        >>> list(overlapping_chunks('ATCG'*4, 4, 2))
+        >>> list(overlapping_chunks('ATCG' * 4, 4, 2))
         [(0, 'ATCGATCG'), (4, 'ATCGATCG'), (8, 'ATCGATCG')]
 
     """
     index = 0
     while index < len(sequence) - 2 * overlap:
         yield index, sequence[index : index + size + 2 * overlap]
         index += size
```

### Comparing `dnacurve-2023.8.30/dnacurve/web.py` & `dnacurve-2024.5.10/dnacurve/web.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python3
 # dnacurve/web.py
 
-# Copyright (c) 2005-2023, Christoph Gohlke
+# Copyright (c) 2005-2024, Christoph Gohlke
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #
 # 1. Redistributions of source code must retain the above copyright notice,
 #    this list of conditions and the following disclaimer.
```

### Comparing `dnacurve-2023.8.30/dnacurve.egg-info/PKG-INFO` & `dnacurve-2024.5.10/dnacurve.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dnacurve
-Version: 2023.8.30
+Version: 2024.5.10
 Summary: DNA curvature analysis
 Home-page: https://www.cgohlke.com
 Author: Christoph Gohlke
 Author-email: cgohlke@cgohlke.com
 License: BSD
 Project-URL: Bug Tracker, https://github.com/cgohlke/dnacurve/issues
 Project-URL: Source Code, https://github.com/cgohlke/dnacurve
@@ -17,28 +17,31 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
-Provides-Extra: all
 License-File: LICENSE
+Requires-Dist: numpy
+Requires-Dist: matplotlib
+Provides-Extra: all
+Requires-Dist: Flask; extra == "all"
 
 DNA curvature analysis
 ======================
 
 Dnacurve is a Python library, console script, and web application to calculate
 the global 3D structure of a B-DNA molecule from its nucleotide sequence
 according to the dinucleotide wedge model. Local bending angles and macroscopic
 curvature are calculated at each nucleotide.
 
 :Author: `Christoph Gohlke <https://www.cgohlke.com>`_
 :License: BSD 3-Clause
-:Version: 2023.8.30
+:Version: 2024.5.10
 :DOI: `10.5281/zenodo.7135499 <https://doi.org/10.5281/zenodo.7135499>`_
 
 Quickstart
 ----------
 
 Install the dnacurve package and all dependencies from the
 `Python Package Index <https://pypi.org/project/dnacurve/>`_::
@@ -60,22 +63,26 @@
 
 Requirements
 ------------
 
 This revision was tested with the following requirements and dependencies
 (other versions may work):
 
-- `CPython <https://www.python.org>`_ 3.9.13, 3.10.11, 3.11.5, 3.12rc
-- `Numpy <https://pypi.org/project/numpy/>`_ 1.25.2
-- `Matplotlib <https://pypi.org/project/matplotlib/>`_ 3.7.2
-- `Flask <https://pypi.org/project/Flask/>`_ 2.3.3 (optional)
+- `CPython <https://www.python.org>`_ 3.9.13, 3.10.11, 3.11.9, 3.12.3
+- `Numpy <https://pypi.org/project/numpy/>`_ 1.26.4
+- `Matplotlib <https://pypi.org/project/matplotlib/>`_ 3.8.4
+- `Flask <https://pypi.org/project/Flask/>`_ 3.0.3 (optional)
 
 Revisions
 ---------
 
+2024.5.10
+
+- Fix mypy errors.
+
 2023.8.30
 
 - Fix linting issues.
 - Add py.typed marker.
 
 2023.4.30
```

### Comparing `dnacurve-2023.8.30/setup.py` & `dnacurve-2024.5.10/setup.py`

 * *Files identical despite different names*

