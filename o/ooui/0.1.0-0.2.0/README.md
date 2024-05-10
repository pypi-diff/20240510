# Comparing `tmp/ooui-0.1.0.tar.gz` & `tmp/ooui-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ooui-0.1.0.tar", last modified: Thu May  9 09:05:31 2024, max compression
+gzip compressed data, was "ooui-0.2.0.tar", last modified: Fri May 10 13:16:14 2024, max compression
```

## Comparing `ooui-0.1.0.tar` & `ooui-0.2.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 ecarreras  (1000) ecarreras  (1000)        0 2024-05-09 09:05:31.415238 ooui-0.1.0/
--rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)     1065 2024-05-06 16:18:58.000000 ooui-0.1.0/LICENSE
--rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)      268 2024-05-09 09:05:31.415238 ooui-0.1.0/PKG-INFO
--rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)       40 2024-05-06 16:18:58.000000 ooui-0.1.0/README.md
-drwxrwxr-x   0 ecarreras  (1000) ecarreras  (1000)        0 2024-05-09 09:05:31.411239 ooui-0.1.0/ooui/
--rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)        0 2024-05-06 16:22:58.000000 ooui-0.1.0/ooui/__init__.py
-drwxrwxr-x   0 ecarreras  (1000) ecarreras  (1000)        0 2024-05-09 09:05:31.415238 ooui-0.1.0/ooui/graph/
--rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)      715 2024-05-09 07:49:02.000000 ooui-0.1.0/ooui/graph/__init__.py
--rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)     2599 2024-05-08 10:59:34.000000 ooui-0.1.0/ooui/graph/axis.py
--rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)      640 2024-05-06 17:25:40.000000 ooui-0.1.0/ooui/graph/base.py
--rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)      444 2024-05-06 17:36:48.000000 ooui-0.1.0/ooui/graph/chart.py
--rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)     3585 2024-05-09 07:54:41.000000 ooui-0.1.0/ooui/graph/fields.py
--rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)     1194 2024-05-06 17:19:53.000000 ooui-0.1.0/ooui/graph/indicator.py
--rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)     6488 2024-05-09 08:58:36.000000 ooui-0.1.0/ooui/graph/processor.py
--rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)     9439 2024-05-08 12:28:50.000000 ooui-0.1.0/ooui/graph/timerange.py
-drwxrwxr-x   0 ecarreras  (1000) ecarreras  (1000)        0 2024-05-09 09:05:31.415238 ooui-0.1.0/ooui/helpers/
--rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)      526 2024-05-06 17:19:46.000000 ooui-0.1.0/ooui/helpers/__init__.py
-drwxrwxr-x   0 ecarreras  (1000) ecarreras  (1000)        0 2024-05-09 09:05:31.411239 ooui-0.1.0/ooui.egg-info/
--rw-r--r--   0 ecarreras  (1000) ecarreras  (1000)      268 2024-05-09 09:05:31.000000 ooui-0.1.0/ooui.egg-info/PKG-INFO
--rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)      381 2024-05-09 09:05:31.000000 ooui-0.1.0/ooui.egg-info/SOURCES.txt
--rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)        1 2024-05-09 09:05:31.000000 ooui-0.1.0/ooui.egg-info/dependency_links.txt
--rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)       25 2024-05-09 09:05:31.000000 ooui-0.1.0/ooui.egg-info/requires.txt
--rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)        5 2024-05-09 09:05:31.000000 ooui-0.1.0/ooui.egg-info/top_level.txt
--rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)       38 2024-05-09 09:05:31.415238 ooui-0.1.0/setup.cfg
--rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)      533 2024-05-08 11:17:49.000000 ooui-0.1.0/setup.py
+drwxrwxr-x   0 ecarreras  (1000) ecarreras  (1000)        0 2024-05-10 13:16:14.842532 ooui-0.2.0/
+-rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)     1065 2024-05-06 16:18:58.000000 ooui-0.2.0/LICENSE
+-rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)      268 2024-05-10 13:16:14.842532 ooui-0.2.0/PKG-INFO
+-rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)       40 2024-05-06 16:18:58.000000 ooui-0.2.0/README.md
+drwxrwxr-x   0 ecarreras  (1000) ecarreras  (1000)        0 2024-05-10 13:16:14.838532 ooui-0.2.0/ooui/
+-rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)        0 2024-05-06 16:22:58.000000 ooui-0.2.0/ooui/__init__.py
+drwxrwxr-x   0 ecarreras  (1000) ecarreras  (1000)        0 2024-05-10 13:16:14.838532 ooui-0.2.0/ooui/graph/
+-rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)      779 2024-05-10 12:16:14.000000 ooui-0.2.0/ooui/graph/__init__.py
+-rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)     2599 2024-05-08 10:59:34.000000 ooui-0.2.0/ooui/graph/axis.py
+-rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)      783 2024-05-10 12:49:23.000000 ooui-0.2.0/ooui/graph/base.py
+-rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)     5632 2024-05-10 12:48:45.000000 ooui-0.2.0/ooui/graph/chart.py
+-rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)     3305 2024-05-10 12:09:54.000000 ooui-0.2.0/ooui/graph/fields.py
+-rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)     1859 2024-05-10 13:12:52.000000 ooui-0.2.0/ooui/graph/indicator.py
+-rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)     2900 2024-05-10 12:48:29.000000 ooui-0.2.0/ooui/graph/processor.py
+-rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)     9439 2024-05-08 12:28:50.000000 ooui-0.2.0/ooui/graph/timerange.py
+drwxrwxr-x   0 ecarreras  (1000) ecarreras  (1000)        0 2024-05-10 13:16:14.842532 ooui-0.2.0/ooui/helpers/
+-rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)      526 2024-05-06 17:19:46.000000 ooui-0.2.0/ooui/helpers/__init__.py
+drwxrwxr-x   0 ecarreras  (1000) ecarreras  (1000)        0 2024-05-10 13:16:14.838532 ooui-0.2.0/ooui.egg-info/
+-rw-r--r--   0 ecarreras  (1000) ecarreras  (1000)      268 2024-05-10 13:16:14.000000 ooui-0.2.0/ooui.egg-info/PKG-INFO
+-rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)      381 2024-05-10 13:16:14.000000 ooui-0.2.0/ooui.egg-info/SOURCES.txt
+-rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)        1 2024-05-10 13:16:14.000000 ooui-0.2.0/ooui.egg-info/dependency_links.txt
+-rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)       25 2024-05-10 13:16:14.000000 ooui-0.2.0/ooui.egg-info/requires.txt
+-rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)        5 2024-05-10 13:16:14.000000 ooui-0.2.0/ooui.egg-info/top_level.txt
+-rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)       38 2024-05-10 13:16:14.842532 ooui-0.2.0/setup.cfg
+-rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)      533 2024-05-10 13:15:09.000000 ooui-0.2.0/setup.py
```

### Comparing `ooui-0.1.0/LICENSE` & `ooui-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ooui-0.1.0/ooui/graph/__init__.py` & `ooui-0.2.0/ooui/graph/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from __future__ import absolute_import, unicode_literals
 from lxml import etree
-from ooui.graph.indicator import GraphIndicator
+from ooui.graph.indicator import GraphIndicator, GraphIndicatorField
 from ooui.graph.chart import GraphChart
 
 
 GRAPH_TYPES = {
     'indicator': GraphIndicator,
+    'indicatorField': GraphIndicatorField,
     'line': GraphChart,
     'pie': GraphChart,
     'bar': GraphChart,
 }
 
 
 def parse_graph(xml):
```

### Comparing `ooui-0.1.0/ooui/graph/axis.py` & `ooui-0.2.0/ooui/graph/axis.py`

 * *Files identical despite different names*

### Comparing `ooui-0.1.0/ooui/graph/base.py` & `ooui-0.2.0/ooui/graph/base.py`

 * *Files 7% similar despite different names*

```diff
@@ -25,7 +25,14 @@
     @property
     def interval(self):
         return self._interval
 
     @property
     def type(self):
         return self._type
+
+    @property
+    def fields(self):
+        return []
+
+    def process(self, values, fields, options=None):
+        raise NotImplementedError
```

### Comparing `ooui-0.1.0/ooui/graph/fields.py` & `ooui-0.2.0/ooui/graph/fields.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,28 +5,15 @@
     """
     Returns a list of fields to retrieve from the ooui
     :param ooui: Graph instance
     :type ooui: ooui.graph.chart.GraphChart
     :return: list of fields to retrieve
     :rtype: list[str]
     """
-    x_field = ooui.x.name
-    fields = [x_field]
-
-    if not ooui.y:
-        return []
-
-    for y in ooui.y:
-        if y.operator != 'count' and y.name not in fields:
-            fields.append(y.name)
-
-        if y.label and y.label not in fields:
-            fields.append(y.label)
-
-    return fields
+    return ooui.fields
 
 
 def get_value_and_label_for_field(fields, values, field_name):
     """
     Retrieve the value and label for a specific field.
 
     :param dict fields: A dictionary containing the field definitions.
```

### Comparing `ooui-0.1.0/ooui/graph/timerange.py` & `ooui-0.2.0/ooui/graph/timerange.py`

 * *Files identical despite different names*

### Comparing `ooui-0.1.0/ooui/helpers/__init__.py` & `ooui-0.2.0/ooui/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `ooui-0.1.0/setup.py` & `ooui-0.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 setup(
     name='ooui',
     description='Open Object User Interface',
     author='GISCE',
     author_email='devel@gisce.net',
     url='https://github.com/gisce/python-ooui',
-    version='0.1.0',
+    version='0.2.0',
     license='MIT',
     long_description='''Open Object User Interface for GISCE-ERP''',
     provides=['ooui'],
     install_requires=[
         'lxml',
         'python-dateutil',
         'six',
```

