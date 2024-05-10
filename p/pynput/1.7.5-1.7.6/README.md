# Comparing `tmp/pynput-1.7.5.tar.gz` & `tmp/pynput-1.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynput-1.7.5.tar", last modified: Fri Nov 19 08:55:19 2021, max compression
+gzip compressed data, was "pynput-1.7.6.tar", last modified: Sat Jan  1 19:57:30 2022, max compression
```

## Comparing `pynput-1.7.5.tar` & `pynput-1.7.6.tar`

### file list

```diff
@@ -1,41 +1,42 @@
-drwxrwxr-x   0 moses     (1000) moses     (1000)        0 2021-11-19 08:55:19.065269 pynput-1.7.5/
--rw-rw-r--   0 moses     (1000) moses     (1000)     7651 2021-02-10 16:50:49.000000 pynput-1.7.5/COPYING.LGPL
--rw-rw-r--   0 moses     (1000) moses     (1000)    29569 2021-11-19 08:55:19.065269 pynput-1.7.5/PKG-INFO
--rw-rw-r--   0 moses     (1000) moses     (1000)      228 2021-11-14 11:58:22.000000 pynput-1.7.5/README.rst
-drwxrwxr-x   0 moses     (1000) moses     (1000)        0 2021-11-19 08:55:19.065269 pynput-1.7.5/lib/
-drwxrwxr-x   0 moses     (1000) moses     (1000)        0 2021-11-19 08:55:19.065269 pynput-1.7.5/lib/pynput/
--rw-rw-r--   0 moses     (1000) moses     (1000)     1334 2021-10-26 13:00:52.000000 pynput-1.7.5/lib/pynput/__init__.py
--rw-rw-r--   0 moses     (1000) moses     (1000)      775 2021-11-19 08:55:11.000000 pynput-1.7.5/lib/pynput/_info.py
-drwxrwxr-x   0 moses     (1000) moses     (1000)        0 2021-11-19 08:55:19.065269 pynput-1.7.5/lib/pynput/_util/
--rw-rw-r--   0 moses     (1000) moses     (1000)    13735 2021-11-14 10:36:25.000000 pynput-1.7.5/lib/pynput/_util/__init__.py
--rw-rw-r--   0 moses     (1000) moses     (1000)     8623 2021-11-14 11:58:54.000000 pynput-1.7.5/lib/pynput/_util/darwin.py
--rw-rw-r--   0 moses     (1000) moses     (1000)     2813 2021-10-26 13:00:52.000000 pynput-1.7.5/lib/pynput/_util/uinput.py
--rw-rw-r--   0 moses     (1000) moses     (1000)    18110 2021-11-14 11:58:54.000000 pynput-1.7.5/lib/pynput/_util/win32.py
--rw-rw-r--   0 moses     (1000) moses     (1000)     2894 2021-10-26 13:00:52.000000 pynput-1.7.5/lib/pynput/_util/win32_vks.py
--rw-rw-r--   0 moses     (1000) moses     (1000)    15234 2021-11-14 11:58:54.000000 pynput-1.7.5/lib/pynput/_util/xorg.py
--rw-rw-r--   0 moses     (1000) moses     (1000)    69338 2021-10-26 13:00:52.000000 pynput-1.7.5/lib/pynput/_util/xorg_keysyms.py
-drwxrwxr-x   0 moses     (1000) moses     (1000)        0 2021-11-19 08:55:19.065269 pynput-1.7.5/lib/pynput/keyboard/
--rw-rw-r--   0 moses     (1000) moses     (1000)     7208 2021-10-26 13:00:52.000000 pynput-1.7.5/lib/pynput/keyboard/__init__.py
--rw-rw-r--   0 moses     (1000) moses     (1000)    21923 2021-11-14 10:36:25.000000 pynput-1.7.5/lib/pynput/keyboard/_base.py
--rw-rw-r--   0 moses     (1000) moses     (1000)    10936 2021-11-14 11:56:05.000000 pynput-1.7.5/lib/pynput/keyboard/_darwin.py
--rw-rw-r--   0 moses     (1000) moses     (1000)      895 2021-10-26 13:00:52.000000 pynput-1.7.5/lib/pynput/keyboard/_dummy.py
--rw-rw-r--   0 moses     (1000) moses     (1000)    14654 2021-11-14 11:58:54.000000 pynput-1.7.5/lib/pynput/keyboard/_uinput.py
--rw-rw-r--   0 moses     (1000) moses     (1000)    10829 2021-11-14 11:58:54.000000 pynput-1.7.5/lib/pynput/keyboard/_win32.py
--rw-rw-r--   0 moses     (1000) moses     (1000)    21885 2021-11-19 08:52:32.000000 pynput-1.7.5/lib/pynput/keyboard/_xorg.py
-drwxrwxr-x   0 moses     (1000) moses     (1000)        0 2021-11-19 08:55:19.065269 pynput-1.7.5/lib/pynput/mouse/
--rw-rw-r--   0 moses     (1000) moses     (1000)     2576 2021-10-26 13:00:52.000000 pynput-1.7.5/lib/pynput/mouse/__init__.py
--rw-rw-r--   0 moses     (1000) moses     (1000)     8438 2021-11-14 10:36:25.000000 pynput-1.7.5/lib/pynput/mouse/_base.py
--rw-rw-r--   0 moses     (1000) moses     (1000)     6735 2021-11-14 11:56:05.000000 pynput-1.7.5/lib/pynput/mouse/_darwin.py
--rw-rw-r--   0 moses     (1000) moses     (1000)      874 2021-10-26 13:00:52.000000 pynput-1.7.5/lib/pynput/mouse/_dummy.py
--rw-rw-r--   0 moses     (1000) moses     (1000)     6827 2021-11-14 10:36:25.000000 pynput-1.7.5/lib/pynput/mouse/_win32.py
--rw-rw-r--   0 moses     (1000) moses     (1000)     5425 2021-11-14 10:36:25.000000 pynput-1.7.5/lib/pynput/mouse/_xorg.py
-drwxrwxr-x   0 moses     (1000) moses     (1000)        0 2021-11-19 08:55:19.065269 pynput-1.7.5/lib/pynput.egg-info/
--rw-rw----   0 moses     (1000) moses     (1000)    29569 2021-11-19 08:55:19.000000 pynput-1.7.5/lib/pynput.egg-info/PKG-INFO
--rw-rw----   0 moses     (1000) moses     (1000)      884 2021-11-19 08:55:19.000000 pynput-1.7.5/lib/pynput.egg-info/SOURCES.txt
--rw-rw----   0 moses     (1000) moses     (1000)        1 2021-11-19 08:55:19.000000 pynput-1.7.5/lib/pynput.egg-info/dependency_links.txt
--rw-rw----   0 moses     (1000) moses     (1000)       47 2017-02-01 21:17:29.000000 pynput-1.7.5/lib/pynput.egg-info/pbr.json
--rw-rw----   0 moses     (1000) moses     (1000)      196 2021-11-19 08:55:19.000000 pynput-1.7.5/lib/pynput.egg-info/requires.txt
--rw-rw----   0 moses     (1000) moses     (1000)        7 2021-11-19 08:55:19.000000 pynput-1.7.5/lib/pynput.egg-info/top_level.txt
--rw-rw----   0 moses     (1000) moses     (1000)        1 2015-10-15 12:32:04.000000 pynput-1.7.5/lib/pynput.egg-info/zip-safe
--rw-rw----   0 moses     (1000) moses     (1000)      184 2021-11-19 08:55:19.065269 pynput-1.7.5/setup.cfg
--rw-rw-r--   0 moses     (1000) moses     (1000)     3709 2021-11-14 11:58:54.000000 pynput-1.7.5/setup.py
+drwxrwxr-x   0 moses     (1000) moses     (1000)        0 2022-01-01 19:57:30.649230 pynput-1.7.6/
+-rw-rw-r--   0 moses     (1000) moses     (1000)     7656 2022-01-01 19:56:27.000000 pynput-1.7.6/COPYING.LGPL
+-rw-rw-r--   0 moses     (1000) moses     (1000)    36798 2022-01-01 19:57:30.649230 pynput-1.7.6/PKG-INFO
+-rw-rw-r--   0 moses     (1000) moses     (1000)      228 2022-01-01 19:56:27.000000 pynput-1.7.6/README.rst
+drwxrwxr-x   0 moses     (1000) moses     (1000)        0 2022-01-01 19:57:30.649230 pynput-1.7.6/lib/
+drwxrwxr-x   0 moses     (1000) moses     (1000)        0 2022-01-01 19:57:30.649230 pynput-1.7.6/lib/pynput/
+-rw-rw-r--   0 moses     (1000) moses     (1000)     1334 2022-01-01 19:56:27.000000 pynput-1.7.6/lib/pynput/__init__.py
+-rw-rw-r--   0 moses     (1000) moses     (1000)      775 2022-01-01 19:57:22.000000 pynput-1.7.6/lib/pynput/_info.py
+drwxrwxr-x   0 moses     (1000) moses     (1000)        0 2022-01-01 19:57:30.649230 pynput-1.7.6/lib/pynput/_util/
+-rw-rw-r--   0 moses     (1000) moses     (1000)    14327 2022-01-01 19:56:27.000000 pynput-1.7.6/lib/pynput/_util/__init__.py
+-rw-rw-r--   0 moses     (1000) moses     (1000)     8654 2022-01-01 19:56:27.000000 pynput-1.7.6/lib/pynput/_util/darwin.py
+-rw-rw-r--   0 moses     (1000) moses     (1000)     1512 2022-01-01 19:56:27.000000 pynput-1.7.6/lib/pynput/_util/darwin_vks.py
+-rw-rw-r--   0 moses     (1000) moses     (1000)     2813 2022-01-01 19:56:27.000000 pynput-1.7.6/lib/pynput/_util/uinput.py
+-rw-rw-r--   0 moses     (1000) moses     (1000)    18110 2022-01-01 19:56:27.000000 pynput-1.7.6/lib/pynput/_util/win32.py
+-rw-rw-r--   0 moses     (1000) moses     (1000)     2894 2022-01-01 19:56:27.000000 pynput-1.7.6/lib/pynput/_util/win32_vks.py
+-rw-rw-r--   0 moses     (1000) moses     (1000)    15103 2022-01-01 19:56:27.000000 pynput-1.7.6/lib/pynput/_util/xorg.py
+-rw-rw-r--   0 moses     (1000) moses     (1000)    69338 2022-01-01 19:56:27.000000 pynput-1.7.6/lib/pynput/_util/xorg_keysyms.py
+drwxrwxr-x   0 moses     (1000) moses     (1000)        0 2022-01-01 19:57:30.649230 pynput-1.7.6/lib/pynput/keyboard/
+-rw-rw-r--   0 moses     (1000) moses     (1000)     7208 2022-01-01 19:56:27.000000 pynput-1.7.6/lib/pynput/keyboard/__init__.py
+-rw-rw-r--   0 moses     (1000) moses     (1000)    22399 2022-01-01 19:56:27.000000 pynput-1.7.6/lib/pynput/keyboard/_base.py
+-rw-rw-r--   0 moses     (1000) moses     (1000)    11314 2022-01-01 19:56:27.000000 pynput-1.7.6/lib/pynput/keyboard/_darwin.py
+-rw-rw-r--   0 moses     (1000) moses     (1000)      895 2022-01-01 19:56:27.000000 pynput-1.7.6/lib/pynput/keyboard/_dummy.py
+-rw-rw-r--   0 moses     (1000) moses     (1000)    14398 2022-01-01 19:56:27.000000 pynput-1.7.6/lib/pynput/keyboard/_uinput.py
+-rw-rw-r--   0 moses     (1000) moses     (1000)    10829 2022-01-01 19:56:27.000000 pynput-1.7.6/lib/pynput/keyboard/_win32.py
+-rw-rw-r--   0 moses     (1000) moses     (1000)    21888 2022-01-01 19:56:27.000000 pynput-1.7.6/lib/pynput/keyboard/_xorg.py
+drwxrwxr-x   0 moses     (1000) moses     (1000)        0 2022-01-01 19:57:30.649230 pynput-1.7.6/lib/pynput/mouse/
+-rw-rw-r--   0 moses     (1000) moses     (1000)     2576 2022-01-01 19:56:27.000000 pynput-1.7.6/lib/pynput/mouse/__init__.py
+-rw-rw-r--   0 moses     (1000) moses     (1000)     8445 2022-01-01 19:56:27.000000 pynput-1.7.6/lib/pynput/mouse/_base.py
+-rw-rw-r--   0 moses     (1000) moses     (1000)     6735 2022-01-01 19:56:27.000000 pynput-1.7.6/lib/pynput/mouse/_darwin.py
+-rw-rw-r--   0 moses     (1000) moses     (1000)      874 2022-01-01 19:56:27.000000 pynput-1.7.6/lib/pynput/mouse/_dummy.py
+-rw-rw-r--   0 moses     (1000) moses     (1000)     6827 2022-01-01 19:56:27.000000 pynput-1.7.6/lib/pynput/mouse/_win32.py
+-rw-rw-r--   0 moses     (1000) moses     (1000)     5425 2022-01-01 19:56:27.000000 pynput-1.7.6/lib/pynput/mouse/_xorg.py
+drwxrwxr-x   0 moses     (1000) moses     (1000)        0 2022-01-01 19:57:30.649230 pynput-1.7.6/lib/pynput.egg-info/
+-rw-rw----   0 moses     (1000) moses     (1000)    36798 2022-01-01 19:57:30.000000 pynput-1.7.6/lib/pynput.egg-info/PKG-INFO
+-rw-rw----   0 moses     (1000) moses     (1000)      915 2022-01-01 19:57:30.000000 pynput-1.7.6/lib/pynput.egg-info/SOURCES.txt
+-rw-rw----   0 moses     (1000) moses     (1000)        1 2022-01-01 19:57:30.000000 pynput-1.7.6/lib/pynput.egg-info/dependency_links.txt
+-rw-rw----   0 moses     (1000) moses     (1000)       47 2017-02-01 21:17:29.000000 pynput-1.7.6/lib/pynput.egg-info/pbr.json
+-rw-rw----   0 moses     (1000) moses     (1000)      196 2022-01-01 19:57:30.000000 pynput-1.7.6/lib/pynput.egg-info/requires.txt
+-rw-rw----   0 moses     (1000) moses     (1000)        7 2022-01-01 19:57:30.000000 pynput-1.7.6/lib/pynput.egg-info/top_level.txt
+-rw-rw----   0 moses     (1000) moses     (1000)        1 2015-10-15 12:32:04.000000 pynput-1.7.6/lib/pynput.egg-info/zip-safe
+-rw-rw----   0 moses     (1000) moses     (1000)      184 2022-01-01 19:57:30.649230 pynput-1.7.6/setup.cfg
+-rw-rw-r--   0 moses     (1000) moses     (1000)     3709 2022-01-01 19:56:27.000000 pynput-1.7.6/setup.py
```

### Comparing `pynput-1.7.5/COPYING.LGPL` & `pynput-1.7.6/COPYING.LGPL`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
                    GNU LESSER GENERAL PUBLIC LICENSE
                        Version 3, 29 June 2007
 
- Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
+ Copyright (C) 2007-2022 Free Software Foundation, Inc. <http://fsf.org/>
  Everyone is permitted to copy and distribute verbatim copies
  of this license document, but changing it is not allowed.
 
 
   This version of the GNU Lesser General Public License incorporates
 the terms and conditions of version 3 of the GNU General Public
 License, supplemented by the additional permissions listed below.
```

### Comparing `pynput-1.7.5/lib/pynput/__init__.py` & `pynput-1.7.6/lib/pynput/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # coding=utf-8
 # pynput
-# Copyright (C) 2015-2021 Moses Palmér
+# Copyright (C) 2015-2022 Moses Palmér
 #
 # This program is free software: you can redistribute it and/or modify it under
 # the terms of the GNU Lesser General Public License as published by the Free
 # Software Foundation, either version 3 of the License, or (at your option) any
 # later version.
 #
 # This program is distributed in the hope that it will be useful, but WITHOUT
```

### Comparing `pynput-1.7.5/lib/pynput/_info.py` & `pynput-1.7.6/lib/pynput/_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # coding=utf-8
 # pystray
-# Copyright (C) 2015-2021 Moses Palmér
+# Copyright (C) 2015-2022 Moses Palmér
 #
 # This program is free software: you can redistribute it and/or modify it under
 # the terms of the GNU Lesser General Public License as published by the Free
 # Software Foundation, either version 3 of the License, or (at your option) any
 # later version.
 #
 # This program is distributed in the hope that it will be useful, but WITHOUT
@@ -12,8 +12,8 @@
 # FOR A PARTICULAR PURPOSE. See the GNU Lesser General Public License for more
 # details.
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 
 __author__ = u'Moses Palmér'
-__version__ = (1, 7, 5)
+__version__ = (1, 7, 6)
```

### Comparing `pynput-1.7.5/lib/pynput/_util/__init__.py` & `pynput-1.7.6/lib/pynput/_util/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # coding=utf-8
 # pynput
-# Copyright (C) 2015-2021 Moses Palmér
+# Copyright (C) 2015-2022 Moses Palmér
 #
 # This program is free software: you can redistribute it and/or modify it under
 # the terms of the GNU Lesser General Public License as published by the Free
 # Software Foundation, either version 3 of the License, or (at your option) any
 # later version.
 #
 # This program is distributed in the hope that it will be useful, but WITHOUT
@@ -78,14 +78,31 @@
             'Try one of the following resolutions:\n\n'
             + '\n\n'.join(
                 ' * {}'.format(s)
                 for s in resolutions))
             if resolutions else '')
 
 
+def prefix(base, cls):
+    """Calculates the prefix to use for platform specific options for a
+    specific class.
+
+    The prefix if the name of the module containing the class that is an
+    immediate subclass of ``base`` among the super classes of ``cls``.
+    """
+    for super_cls in filter(
+            lambda cls: issubclass(cls, base),
+            cls.__mro__[1:]):
+        if super_cls is base:
+            return cls.__module__.rsplit('.', 1)[-1][1:] + '_'
+        else:
+            result = prefix(base, super_cls)
+            if result is not None:
+                return result
+
 
 class AbstractListener(threading.Thread):
     """A class implementing the basic behaviour for event listeners.
 
     Instances of this class can be used as context managers. This is equivalent
     to the following code::
```

### Comparing `pynput-1.7.5/lib/pynput/_util/darwin.py` & `pynput-1.7.6/lib/pynput/_util/darwin.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # coding=utf-8
 # pynput
-# Copyright (C) 2015-2021 Moses Palmér
+# Copyright (C) 2015-2022 Moses Palmér
 #
 # This program is free software: you can redistribute it and/or modify it under
 # the terms of the GNU Lesser General Public License as published by the Free
 # Software Foundation, either version 3 of the License, or (at your option) any
 # later version.
 #
 # This program is distributed in the hope that it will be useful, but WITHOUT
@@ -38,15 +38,15 @@
 def _wrap_value(value):
     """Converts a pointer to a *Python objc* value.
 
     :param value: The pointer to convert.
 
     :return: a wrapped value
     """
-    return objc.objc_object(c_void_p=value)
+    return objc.objc_object(c_void_p=value) if value is not None else None
 
 
 @contextlib.contextmanager
 def _wrapped(value):
     """A context manager that converts a raw pointer to a *Python objc* value.
 
     When the block is exited, the value is released.
```

### Comparing `pynput-1.7.5/lib/pynput/_util/uinput.py` & `pynput-1.7.6/lib/pynput/_util/uinput.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # coding=utf-8
 # pynput
-# Copyright (C) 2015-2021 Moses Palmér
+# Copyright (C) 2015-2022 Moses Palmér
 #
 # This program is free software: you can redistribute it and/or modify it under
 # the terms of the GNU Lesser General Public License as published by the Free
 # Software Foundation, either version 3 of the License, or (at your option) any
 # later version.
 #
 # This program is distributed in the hope that it will be useful, but WITHOUT
```

### Comparing `pynput-1.7.5/lib/pynput/_util/win32.py` & `pynput-1.7.6/lib/pynput/_util/win32.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # coding=utf-8
 # pynput
-# Copyright (C) 2015-2021 Moses Palmér
+# Copyright (C) 2015-2022 Moses Palmér
 #
 # This program is free software: you can redistribute it and/or modify it under
 # the terms of the GNU Lesser General Public License as published by the Free
 # Software Foundation, either version 3 of the License, or (at your option) any
 # later version.
 #
 # This program is distributed in the hope that it will be useful, but WITHOUT
```

### Comparing `pynput-1.7.5/lib/pynput/_util/win32_vks.py` & `pynput-1.7.6/lib/pynput/_util/win32_vks.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # coding: utf-8
 # pynput
-# Copyright (C) 2015-2021 Moses Palmér
+# Copyright (C) 2015-2022 Moses Palmér
 #
 # This program is free software: you can redistribute it and/or modify it under
 # the terms of the GNU Lesser General Public License as published by the Free
 # Software Foundation, either version 3 of the License, or (at your option) any
 # later version.
 #
 # This program is distributed in the hope that it will be useful, but WITHOUT
```

### Comparing `pynput-1.7.5/lib/pynput/_util/xorg.py` & `pynput-1.7.6/lib/pynput/_util/xorg.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # coding=utf-8
 # pynput
-# Copyright (C) 2015-2021 Moses Palmér
+# Copyright (C) 2015-2022 Moses Palmér
 #
 # This program is free software: you can redistribute it and/or modify it under
 # the terms of the GNU Lesser General Public License as published by the Free
 # Software Foundation, either version 3 of the License, or (at your option) any
 # later version.
 #
 # This program is distributed in the hope that it will be useful, but WITHOUT
@@ -419,21 +419,17 @@
             self._display_stop.close()
             self._display_record.close()
         # pylint: enable=W0702
 
     def _stop_platform(self):
         if not hasattr(self, '_context'):
             self.wait()
-        # pylint: disable=W0702; we must ignore errors
-        try:
-            with display_manager(self._display_record) as dm:
-                dm.record_disable_context(self._context)
-        except:
-            pass
-        # pylint: enable=W0702
+
+        # Do this asynchronously to avoid deadlocks
+        self._display_record.record_disable_context(self._context)
 
     def _suppress_start(self, display):
         """Starts suppressing events.
 
         :param Xlib.display.Display display: The display for which to suppress
             events.
         """
```

### Comparing `pynput-1.7.5/lib/pynput/_util/xorg_keysyms.py` & `pynput-1.7.6/lib/pynput/_util/xorg_keysyms.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # coding: utf-8
 # pynput
-# Copyright (C) 2015-2021 Moses Palmér
+# Copyright (C) 2015-2022 Moses Palmér
 #
 # This program is free software: you can redistribute it and/or modify it under
 # the terms of the GNU Lesser General Public License as published by the Free
 # Software Foundation, either version 3 of the License, or (at your option) any
 # later version.
 #
 # This program is distributed in the hope that it will be useful, but WITHOUT
```

### Comparing `pynput-1.7.5/lib/pynput/keyboard/__init__.py` & `pynput-1.7.6/lib/pynput/keyboard/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # coding=utf-8
 # pynput
-# Copyright (C) 2015-2021 Moses Palmér
+# Copyright (C) 2015-2022 Moses Palmér
 #
 # This program is free software: you can redistribute it and/or modify it under
 # the terms of the GNU Lesser General Public License as published by the Free
 # Software Foundation, either version 3 of the License, or (at your option) any
 # later version.
 #
 # This program is distributed in the hope that it will be useful, but WITHOUT
```

### Comparing `pynput-1.7.5/lib/pynput/keyboard/_base.py` & `pynput-1.7.6/lib/pynput/keyboard/_base.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # coding=utf-8
 # pynput
-# Copyright (C) 2015-2021 Moses Palmér
+# Copyright (C) 2015-2022 Moses Palmér
 #
 # This program is free software: you can redistribute it and/or modify it under
 # the terms of the GNU Lesser General Public License as published by the Free
 # Software Foundation, either version 3 of the License, or (at your option) any
 # later version.
 #
 # This program is distributed in the hope that it will be useful, but WITHOUT
@@ -27,15 +27,15 @@
 import contextlib
 import enum
 import threading
 import unicodedata
 
 import six
 
-from pynput._util import AbstractListener
+from pynput._util import AbstractListener, prefix
 from pynput import _logger
 
 
 class KeyCode(object):
     """
     A :class:`KeyCode` represents the description of a key code used by the
     operating system.
@@ -663,47 +663,55 @@
         :class:`KeyCode`, a :class:`Key` or ``None`` if the key is unknown.
 
     :param bool suppress: Whether to suppress events. Setting this to ``True``
         will prevent the input events from being passed to the rest of the
         system.
 
     :param kwargs: Any non-standard platform dependent options. These should be
-        prefixed with the platform name thus: ``darwin_``, ``xorg_`` or
-        ``win32_``.
+        prefixed with the platform name thus: ``darwin_``, ``uinput_``,
+        ``xorg_`` or ``win32_``.
 
         Supported values are:
 
         ``darwin_intercept``
             A callable taking the arguments ``(event_type, event)``, where
             ``event_type`` is ``Quartz.kCGEventKeyDown`` or
             ``Quartz.kCGEventKeyDown``, and ``event`` is a ``CGEventRef``.
 
             This callable can freely modify the event using functions like
             ``Quartz.CGEventSetIntegerValueField``. If this callable does not
             return the event, the event is suppressed system wide.
 
+        ``uinput_device_paths``
+            A list of device paths.
+
+            If this is specified, *pynput* will limit the number of devices
+            checked for the capabilities needed to those passed, otherwise all
+            system devices will be used. Passing this might be required if an
+            incorrect device is chosen.
+
         ``win32_event_filter``
             A callable taking the arguments ``(msg, data)``, where ``msg`` is
             the current message, and ``data`` associated data as a
             `KBDLLHOOKSTRUCT <https://docs.microsoft.com/en-gb/windows/win32/api/winuser/ns-winuser-kbdllhookstruct>`_.
 
             If this callback returns ``False``, the event will not be
             propagated to the listener callback.
 
             If ``self.suppress_event()`` is called, the event is suppressed
             system wide.
     """
     def __init__(self, on_press=None, on_release=None, suppress=False,
                  **kwargs):
         self._log = _logger(self.__class__)
-        prefix = self.__class__.__module__.rsplit('.', 1)[-1][1:] + '_'
+        option_prefix = prefix(Listener, self.__class__)
         self._options = {
-            key[len(prefix):]: value
+            key[len(option_prefix):]: value
             for key, value in kwargs.items()
-            if key.startswith(prefix)}
+            if key.startswith(option_prefix)}
         super(Listener, self).__init__(
             on_press=on_press, on_release=on_release, suppress=suppress)
 # pylint: enable=W0223
 
     def canonical(self, key):
         """Performs normalisation of a key.
 
@@ -721,9 +729,11 @@
         :rtype: Key or KeyCode
         """
         from pynput.keyboard import Key, KeyCode, _NORMAL_MODIFIERS
         if isinstance(key, KeyCode) and key.char is not None:
             return KeyCode.from_char(key.char.lower())
         elif isinstance(key, Key) and key.value in _NORMAL_MODIFIERS:
             return _NORMAL_MODIFIERS[key.value]
+        elif isinstance(key, Key) and key.value.vk is not None:
+            return KeyCode.from_vk(key.value.vk)
         else:
             return key
```

### Comparing `pynput-1.7.5/lib/pynput/keyboard/_darwin.py` & `pynput-1.7.6/lib/pynput/keyboard/_darwin.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # coding=utf-8
 # pynput
-# Copyright (C) 2015-2021 Moses Palmér
+# Copyright (C) 2015-2022 Moses Palmér
 #
 # This program is free software: you can redistribute it and/or modify it under
 # the terms of the GNU Lesser General Public License as published by the Free
 # Software Foundation, either version 3 of the License, or (at your option) any
 # later version.
 #
 # This program is distributed in the hope that it will be useful, but WITHOUT
@@ -28,14 +28,15 @@
 
 import Quartz
 
 from pynput._util.darwin import (
     get_unicode_to_keycode_map,
     keycode_context,
     ListenerMixin)
+from pynput._util.darwin_vks import SYMBOLS
 from . import _base
 
 
 # From hidsystem/ev_keymap.h
 NX_KEYTYPE_PLAY = 16
 NX_KEYTYPE_MUTE = 7
 NX_KEYTYPE_SOUND_DOWN = 1
@@ -325,12 +326,20 @@
         key = (vk, is_media)
         if key in self._SPECIAL_KEYS:
             return self._SPECIAL_KEYS[key]
 
         # ...then try characters...
         length, chars = Quartz.CGEventKeyboardGetUnicodeString(
             event, 100, None, None)
-        if length > 0:
+        try:
+            printable = chars.isprintable()
+        except AttributeError:
+            printable = chars.isalnum()
+        if not printable and vk in SYMBOLS \
+                and Quartz.CGEventGetFlags(event) \
+                & Quartz.kCGEventFlagMaskControl:
+            return KeyCode.from_char(SYMBOLS[vk], vk=vk)
+        elif length > 0:
             return KeyCode.from_char(chars, vk=vk)
 
         # ...and fall back on a virtual key code
         return KeyCode.from_vk(vk)
```

### Comparing `pynput-1.7.5/lib/pynput/keyboard/_dummy.py` & `pynput-1.7.6/lib/pynput/keyboard/_dummy.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # coding=utf-8
 # pynput
-# Copyright (C) 2015-2021 Moses Palmér
+# Copyright (C) 2015-2022 Moses Palmér
 #
 # This program is free software: you can redistribute it and/or modify it under
 # the terms of the GNU Lesser General Public License as published by the Free
 # Software Foundation, either version 3 of the License, or (at your option) any
 # later version.
 #
 # This program is distributed in the hope that it will be useful, but WITHOUT
```

### Comparing `pynput-1.7.5/lib/pynput/keyboard/_uinput.py` & `pynput-1.7.6/lib/pynput/keyboard/_uinput.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # coding=utf-8
 # pynput
-# Copyright (C) 2015-2021 Moses Palmér
+# Copyright (C) 2015-2022 Moses Palmér
 #
 # This program is free software: you can redistribute it and/or modify it under
 # the terms of the GNU Lesser General Public License as published by the Free
 # Software Foundation, either version 3 of the License, or (at your option) any
 # later version.
 #
 # This program is distributed in the hope that it will be useful, but WITHOUT
@@ -215,26 +215,20 @@
 
         :param int vk: The virtual key code.
 
         :param set modifiers: A set of modifiers.
 
         :return: a mapped key
 
-        :raises ValueError: if ``modifiers`` contains keys other than
-            :attr:`Key.shift` and :attr:`Key.alt_gr`
-
         :raises KeyError: if ``vk`` is an unknown key
         """
-        if not {Key.shift, Key.alt_gr}.issuperset(modifiers):
-            raise ValueError(modifiers)
-        else:
-            return self._vk_table[vk][
-                0
-                | (1 if Key.shift in modifiers else 0)
-                | (2 if Key.alt_gr in modifiers else 0)]
+        return self._vk_table[vk][
+            0
+            | (1 if Key.shift in modifiers else 0)
+            | (2 if Key.alt_gr in modifiers else 0)]
 
     def for_char(self, char):
         """Reads a virtual key code and modifier state for a character.
 
         :param str char: The character.
 
         :return: the tuple ``(vk, modifiers)``
```

### Comparing `pynput-1.7.5/lib/pynput/keyboard/_win32.py` & `pynput-1.7.6/lib/pynput/keyboard/_win32.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # coding=utf-8
 # pynput
-# Copyright (C) 2015-2021 Moses Palmér
+# Copyright (C) 2015-2022 Moses Palmér
 #
 # This program is free software: you can redistribute it and/or modify it under
 # the terms of the GNU Lesser General Public License as published by the Free
 # Software Foundation, either version 3 of the License, or (at your option) any
 # later version.
 #
 # This program is distributed in the hope that it will be useful, but WITHOUT
```

### Comparing `pynput-1.7.5/lib/pynput/keyboard/_xorg.py` & `pynput-1.7.6/lib/pynput/keyboard/_xorg.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # coding=utf-8
 # pynput
-# Copyright (C) 2015-2021 Moses Palmér
+# Copyright (C) 2015-2022 Moses Palmér
 #
 # This program is free software: you can redistribute it and/or modify it under
 # the terms of the GNU Lesser General Public License as published by the Free
 # Software Foundation, either version 3 of the License, or (at your option) any
 # later version.
 #
 # This program is distributed in the hope that it will be useful, but WITHOUT
@@ -232,16 +232,16 @@
         keysym = self._keysym(key)
 
         # Make sure to verify that the key was resolved
         if keysym is None:
             raise self.InvalidKeyException(key)
 
         # If the key has a virtual key code, use that immediately with
-        # fake_input; fake input,being an X server extension, has access to more
-        # internal state that we
+        # fake_input; fake input,being an X server extension, has access to
+        # more internal state that we do
         if key.vk is not None:
             with display_manager(self._display) as dm:
                 Xlib.ext.xtest.fake_input(
                     dm,
                     Xlib.X.KeyPress if is_press else Xlib.X.KeyRelease,
                     dm.keysym_to_keycode(key.vk))
```

### Comparing `pynput-1.7.5/lib/pynput/mouse/__init__.py` & `pynput-1.7.6/lib/pynput/mouse/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # coding=utf-8
 # pynput
-# Copyright (C) 2015-2021 Moses Palmér
+# Copyright (C) 2015-2022 Moses Palmér
 #
 # This program is free software: you can redistribute it and/or modify it under
 # the terms of the GNU Lesser General Public License as published by the Free
 # Software Foundation, either version 3 of the License, or (at your option) any
 # later version.
 #
 # This program is distributed in the hope that it will be useful, but WITHOUT
```

### Comparing `pynput-1.7.5/lib/pynput/mouse/_base.py` & `pynput-1.7.6/lib/pynput/mouse/_base.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # coding=utf-8
 # pynput
-# Copyright (C) 2015-2021 Moses Palmér
+# Copyright (C) 2015-2022 Moses Palmér
 #
 # This program is free software: you can redistribute it and/or modify it under
 # the terms of the GNU Lesser General Public License as published by the Free
 # Software Foundation, either version 3 of the License, or (at your option) any
 # later version.
 #
 # This program is distributed in the hope that it will be useful, but WITHOUT
@@ -22,15 +22,15 @@
 """
 
 # pylint: disable=R0903
 # We implement stubs
 
 import enum
 
-from pynput._util import AbstractListener
+from pynput._util import AbstractListener, prefix
 from pynput import _logger
 
 
 class Button(enum.Enum):
     """The various buttons.
 
     The actual values for these items differ between platforms. Some
@@ -248,16 +248,16 @@
 
             If ``self.suppress_event()`` is called, the event is suppressed
             system wide.
     """
     def __init__(self, on_move=None, on_click=None, on_scroll=None,
                  suppress=False, **kwargs):
         self._log = _logger(self.__class__)
-        prefix = self.__class__.__module__.rsplit('.', 1)[-1][1:] + '_'
+        option_prefix = prefix(Listener, self.__class__)
         self._options = {
-            key[len(prefix):]: value
+            key[len(option_prefix):]: value
             for key, value in kwargs.items()
-            if key.startswith(prefix)}
+            if key.startswith(option_prefix)}
         super(Listener, self).__init__(
             on_move=on_move, on_click=on_click, on_scroll=on_scroll,
             suppress=suppress)
 # pylint: enable=W0223
```

### Comparing `pynput-1.7.5/lib/pynput/mouse/_darwin.py` & `pynput-1.7.6/lib/pynput/mouse/_darwin.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # coding=utf-8
 # pynput
-# Copyright (C) 2015-2021 Moses Palmér
+# Copyright (C) 2015-2022 Moses Palmér
 #
 # This program is free software: you can redistribute it and/or modify it under
 # the terms of the GNU Lesser General Public License as published by the Free
 # Software Foundation, either version 3 of the License, or (at your option) any
 # later version.
 #
 # This program is distributed in the hope that it will be useful, but WITHOUT
```

### Comparing `pynput-1.7.5/lib/pynput/mouse/_dummy.py` & `pynput-1.7.6/lib/pynput/mouse/_dummy.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # pynput
-# Copyright (C) 2015-2021 Moses Palmér
+# Copyright (C) 2015-2022 Moses Palmér
 #
 # This program is free software: you can redistribute it and/or modify it under
 # the terms of the GNU Lesser General Public License as published by the Free
 # Software Foundation, either version 3 of the License, or (at your option) any
 # later version.
 #
 # This program is distributed in the hope that it will be useful, but WITHOUT
```

### Comparing `pynput-1.7.5/lib/pynput/mouse/_win32.py` & `pynput-1.7.6/lib/pynput/mouse/_win32.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # coding=utf-8
 # pynput
-# Copyright (C) 2015-2021 Moses Palmér
+# Copyright (C) 2015-2022 Moses Palmér
 #
 # This program is free software: you can redistribute it and/or modify it under
 # the terms of the GNU Lesser General Public License as published by the Free
 # Software Foundation, either version 3 of the License, or (at your option) any
 # later version.
 #
 # This program is distributed in the hope that it will be useful, but WITHOUT
```

### Comparing `pynput-1.7.5/lib/pynput/mouse/_xorg.py` & `pynput-1.7.6/lib/pynput/mouse/_xorg.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # coding=utf-8
 # pynput
-# Copyright (C) 2015-2021 Moses Palmér
+# Copyright (C) 2015-2022 Moses Palmér
 #
 # This program is free software: you can redistribute it and/or modify it under
 # the terms of the GNU Lesser General Public License as published by the Free
 # Software Foundation, either version 3 of the License, or (at your option) any
 # later version.
 #
 # This program is distributed in the hope that it will be useful, but WITHOUT
```

### Comparing `pynput-1.7.5/lib/pynput.egg-info/SOURCES.txt` & `pynput-1.7.6/lib/pynput.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 lib/pynput.egg-info/dependency_links.txt
 lib/pynput.egg-info/pbr.json
 lib/pynput.egg-info/requires.txt
 lib/pynput.egg-info/top_level.txt
 lib/pynput.egg-info/zip-safe
 lib/pynput/_util/__init__.py
 lib/pynput/_util/darwin.py
+lib/pynput/_util/darwin_vks.py
 lib/pynput/_util/uinput.py
 lib/pynput/_util/win32.py
 lib/pynput/_util/win32_vks.py
 lib/pynput/_util/xorg.py
 lib/pynput/_util/xorg_keysyms.py
 lib/pynput/keyboard/__init__.py
 lib/pynput/keyboard/_base.py
```

### Comparing `pynput-1.7.5/setup.py` & `pynput-1.7.6/setup.py`

 * *Files identical despite different names*

