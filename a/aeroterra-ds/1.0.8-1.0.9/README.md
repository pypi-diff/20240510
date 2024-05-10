# Comparing `tmp/aeroterra_ds-1.0.8.tar.gz` & `tmp/aeroterra_ds-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aeroterra_ds-1.0.8.tar", last modified: Mon Apr 22 14:14:10 2024, max compression
+gzip compressed data, was "aeroterra_ds-1.0.9.tar", last modified: Mon Apr 22 20:51:44 2024, max compression
```

## Comparing `aeroterra_ds-1.0.8.tar` & `aeroterra_ds-1.0.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-04-22 14:14:10.944442 aeroterra_ds-1.0.8/
--rw-rw-rw-   0        0        0     1306 2024-04-22 14:14:10.944442 aeroterra_ds-1.0.8/PKG-INFO
--rw-rw-rw-   0        0        0      835 2024-04-19 19:51:22.000000 aeroterra_ds-1.0.8/README.md
--rw-rw-rw-   0        0        0       42 2024-04-22 14:14:10.944442 aeroterra_ds-1.0.8/setup.cfg
--rw-rw-rw-   0        0        0      888 2024-04-22 14:14:07.000000 aeroterra_ds-1.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-22 14:14:10.923410 aeroterra_ds-1.0.8/src/
-drwxrwxrwx   0        0        0        0 2024-04-22 14:14:10.932930 aeroterra_ds-1.0.8/src/aeroterra_ds.egg-info/
--rw-rw-rw-   0        0        0     1306 2024-04-22 14:14:10.000000 aeroterra_ds-1.0.8/src/aeroterra_ds.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      453 2024-04-22 14:14:10.000000 aeroterra_ds-1.0.8/src/aeroterra_ds.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-22 14:14:10.000000 aeroterra_ds-1.0.8/src/aeroterra_ds.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       62 2024-04-22 14:14:10.000000 aeroterra_ds-1.0.8/src/aeroterra_ds.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-04-22 14:14:10.000000 aeroterra_ds-1.0.8/src/aeroterra_ds.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-22 14:14:10.935932 aeroterra_ds-1.0.8/src/geometry/
--rw-rw-rw-   0        0        0       53 2024-04-19 19:51:19.000000 aeroterra_ds-1.0.8/src/geometry/__init__.py
--rw-rw-rw-   0        0        0     2908 2024-04-19 15:50:56.000000 aeroterra_ds-1.0.8/src/geometry/change_crs.py
--rw-rw-rw-   0        0        0     5752 2024-04-19 19:51:29.000000 aeroterra_ds-1.0.8/src/geometry/geometry.py
-drwxrwxrwx   0        0        0        0 2024-04-22 14:14:10.943441 aeroterra_ds-1.0.8/src/layers/
--rw-rw-rw-   0        0        0       53 2024-04-19 18:38:17.000000 aeroterra_ds-1.0.8/src/layers/__init__.py
--rw-rw-rw-   0        0        0     1405 2024-04-18 20:25:51.000000 aeroterra_ds-1.0.8/src/layers/common.py
--rw-rw-rw-   0        0        0      466 2024-04-18 20:25:50.000000 aeroterra_ds-1.0.8/src/layers/constants.py
--rw-rw-rw-   0        0        0     3096 2024-04-19 19:15:15.000000 aeroterra_ds-1.0.8/src/layers/fields.py
--rw-rw-rw-   0        0        0    10632 2024-04-19 20:58:06.000000 aeroterra_ds-1.0.8/src/layers/layers.py
--rw-rw-rw-   0        0        0     4125 2024-04-22 14:13:36.000000 aeroterra_ds-1.0.8/src/layers/properties.py
--rw-rw-rw-   0        0        0     2323 2024-04-18 20:36:51.000000 aeroterra_ds-1.0.8/src/layers/symbology.py
+drwxrwxrwx   0        0        0        0 2024-04-22 20:51:44.642631 aeroterra_ds-1.0.9/
+-rw-rw-rw-   0        0        0     1306 2024-04-22 20:51:44.642631 aeroterra_ds-1.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      835 2024-04-19 19:51:22.000000 aeroterra_ds-1.0.9/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-22 20:51:44.642631 aeroterra_ds-1.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      888 2024-04-22 20:51:40.000000 aeroterra_ds-1.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-22 20:51:44.614255 aeroterra_ds-1.0.9/src/
+drwxrwxrwx   0        0        0        0 2024-04-22 20:51:44.630347 aeroterra_ds-1.0.9/src/aeroterra_ds.egg-info/
+-rw-rw-rw-   0        0        0     1306 2024-04-22 20:51:44.000000 aeroterra_ds-1.0.9/src/aeroterra_ds.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      453 2024-04-22 20:51:44.000000 aeroterra_ds-1.0.9/src/aeroterra_ds.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-22 20:51:44.000000 aeroterra_ds-1.0.9/src/aeroterra_ds.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       62 2024-04-22 20:51:44.000000 aeroterra_ds-1.0.9/src/aeroterra_ds.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-04-22 20:51:44.000000 aeroterra_ds-1.0.9/src/aeroterra_ds.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-22 20:51:44.634165 aeroterra_ds-1.0.9/src/geometry/
+-rw-rw-rw-   0        0        0       53 2024-04-19 19:51:19.000000 aeroterra_ds-1.0.9/src/geometry/__init__.py
+-rw-rw-rw-   0        0        0     4193 2024-04-22 20:51:04.000000 aeroterra_ds-1.0.9/src/geometry/change_crs.py
+-rw-rw-rw-   0        0        0     5752 2024-04-19 19:51:29.000000 aeroterra_ds-1.0.9/src/geometry/geometry.py
+drwxrwxrwx   0        0        0        0 2024-04-22 20:51:44.641219 aeroterra_ds-1.0.9/src/layers/
+-rw-rw-rw-   0        0        0       53 2024-04-19 18:38:17.000000 aeroterra_ds-1.0.9/src/layers/__init__.py
+-rw-rw-rw-   0        0        0     1405 2024-04-18 20:25:51.000000 aeroterra_ds-1.0.9/src/layers/common.py
+-rw-rw-rw-   0        0        0      466 2024-04-18 20:25:50.000000 aeroterra_ds-1.0.9/src/layers/constants.py
+-rw-rw-rw-   0        0        0     3096 2024-04-19 19:15:15.000000 aeroterra_ds-1.0.9/src/layers/fields.py
+-rw-rw-rw-   0        0        0    10632 2024-04-19 20:58:06.000000 aeroterra_ds-1.0.9/src/layers/layers.py
+-rw-rw-rw-   0        0        0     4125 2024-04-22 14:26:14.000000 aeroterra_ds-1.0.9/src/layers/properties.py
+-rw-rw-rw-   0        0        0     2323 2024-04-18 20:36:51.000000 aeroterra_ds-1.0.9/src/layers/symbology.py
```

### Comparing `aeroterra_ds-1.0.8/PKG-INFO` & `aeroterra_ds-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aeroterra_ds
-Version: 1.0.8
+Version: 1.0.9
 Summary: Python Functions To Work With GeoSpatial Data & ArcGis in a simpler way
 Home-page: https://example.com
 Author: Data Science
 Author-email: aeroterra_ds@aeroterra.com
 Keywords: arcgis
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `aeroterra_ds-1.0.8/README.md` & `aeroterra_ds-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `aeroterra_ds-1.0.8/setup.py` & `aeroterra_ds-1.0.9/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='aeroterra_ds',
-    version='1.0.8',
+    version='1.0.9',
     author='Data Science',
     author_email='aeroterra_ds@aeroterra.com',
     description='Python Functions To Work With GeoSpatial Data & ArcGis in a simpler way',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://example.com',
     package_dir={'': "src"},
```

### Comparing `aeroterra_ds-1.0.8/src/aeroterra_ds.egg-info/PKG-INFO` & `aeroterra_ds-1.0.9/src/aeroterra_ds.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aeroterra-ds
-Version: 1.0.8
+Version: 1.0.9
 Summary: Python Functions To Work With GeoSpatial Data & ArcGis in a simpler way
 Home-page: https://example.com
 Author: Data Science
 Author-email: aeroterra_ds@aeroterra.com
 Keywords: arcgis
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `aeroterra_ds-1.0.8/src/geometry/change_crs.py` & `aeroterra_ds-1.0.9/src/geometry/change_crs.py`

 * *Files 25% similar despite different names*

```diff
@@ -46,21 +46,57 @@
         transformed_interiors = [[transformador.transform(v[0], v[1]) for v in hole.coords] for hole in pol.interiors]
         
         transformed_polygon = Polygon(transformed_exterior, transformed_interiors)
         multi_new.append(transformed_polygon)
     
     return unary_union(multi_new)
 
+
+def change_crs_linestring(line, crs_fuente, crs_final):
+    if not isinstance(line, LineString):
+        raise Exception("Geometry Must Be A LineString")
+    src_origen = pyproj.CRS(crs_fuente)
+    src_destino = pyproj.CRS(crs_final)
+    transformador = pyproj.Transformer.from_crs(src_origen, src_destino, always_xy=True)
+
+    points = []
+    for point in line.coords:
+        points.append(transformador.transform(point[0], point[1]))
+    
+    return LineString(points)
+
+
+def change_crs_multilinestring(multiline, crs_fuente, crs_final):
+    if not isinstance(multiline, MultiLineString):
+        raise Exception("Geometry Must Be A MultiLineString")
+    src_origen = pyproj.CRS(crs_fuente)
+    src_destino = pyproj.CRS(crs_final)
+    transformador = pyproj.Transformer.from_crs(src_origen, src_destino, always_xy=True)
+
+    lines = []
+    for line in multiline.geoms:
+        points = []
+        for point in line.coords:
+            points.append(transformador.transform(point[0], point[1]))
+        lines.append(LineString(points))
+    
+    return MultiLineString(lines)
+
+
 def change_crs(item, src_crs, dst_crs):
     if isinstance(item, Point):
         return change_crs_point(item, src_crs, dst_crs)
     if isinstance(item, Polygon):
         return change_crs_polygon(item, src_crs, dst_crs)
     if isinstance(item, MultiPolygon):
         return change_crs_multipolygon(item, src_crs, dst_crs)
+    if isinstance(item, LineString):
+        return change_crs_linestring(item, src_crs, dst_crs)
+    if isinstance(item, MultiLineString):
+        return change_crs_multilinestring(item, src_crs, dst_crs)
     if isinstance(item, tuple) and len(item) == 2:
         return change_crs_tuple_point(item, src_crs, dst_crs)
     
     if isinstance(item, list):
         new_list = item.copy()
         for i, sub_item in enumerate(item):
             new_list[i] = change_crs(sub_item, src_crs, dst_crs)
```

### Comparing `aeroterra_ds-1.0.8/src/geometry/geometry.py` & `aeroterra_ds-1.0.9/src/geometry/geometry.py`

 * *Files identical despite different names*

### Comparing `aeroterra_ds-1.0.8/src/layers/common.py` & `aeroterra_ds-1.0.9/src/layers/common.py`

 * *Files identical despite different names*

### Comparing `aeroterra_ds-1.0.8/src/layers/fields.py` & `aeroterra_ds-1.0.9/src/layers/fields.py`

 * *Files identical despite different names*

### Comparing `aeroterra_ds-1.0.8/src/layers/layers.py` & `aeroterra_ds-1.0.9/src/layers/layers.py`

 * *Files identical despite different names*

### Comparing `aeroterra_ds-1.0.8/src/layers/properties.py` & `aeroterra_ds-1.0.9/src/layers/properties.py`

 * *Files identical despite different names*

### Comparing `aeroterra_ds-1.0.8/src/layers/symbology.py` & `aeroterra_ds-1.0.9/src/layers/symbology.py`

 * *Files identical despite different names*

