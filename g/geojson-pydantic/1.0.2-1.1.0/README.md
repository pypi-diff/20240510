# Comparing `tmp/geojson_pydantic-1.0.2.tar.gz` & `tmp/geojson_pydantic-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geojson_pydantic-1.0.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "geojson_pydantic-1.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `geojson_pydantic-1.0.2.tar` & `geojson_pydantic-1.1.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      220 2024-01-16 18:12:54.639849 geojson_pydantic-1.0.2/.bumpversion.cfg
--rw-r--r--   0        0        0     1173 2024-01-16 18:12:54.639849 geojson_pydantic-1.0.2/.gitignore
--rw-r--r--   0        0        0      797 2024-01-16 18:12:54.639849 geojson_pydantic-1.0.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1073 2024-01-16 18:12:54.639849 geojson_pydantic-1.0.2/LICENSE
--rw-r--r--   0        0        0     2892 2024-01-16 18:12:54.639849 geojson_pydantic-1.0.2/README.md
--rw-r--r--   0        0        0      448 2024-01-16 18:12:54.639849 geojson_pydantic-1.0.2/geojson_pydantic/__init__.py
--rw-r--r--   0        0        0     2925 2024-01-16 18:12:54.639849 geojson_pydantic-1.0.2/geojson_pydantic/base.py
--rw-r--r--   0        0        0     1564 2024-01-16 18:12:54.639849 geojson_pydantic-1.0.2/geojson_pydantic/features.py
--rw-r--r--   0        0        0    10662 2024-01-16 18:12:54.639849 geojson_pydantic-1.0.2/geojson_pydantic/geometries.py
--rw-r--r--   0        0        0        0 2024-01-16 18:12:54.639849 geojson_pydantic-1.0.2/geojson_pydantic/py.typed
--rw-r--r--   0        0        0      647 2024-01-16 18:12:54.639849 geojson_pydantic-1.0.2/geojson_pydantic/types.py
--rw-r--r--   0        0        0     2254 2024-01-16 18:12:54.639849 geojson_pydantic-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     4053 1970-01-01 00:00:00.000000 geojson_pydantic-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0      220 2024-05-10 14:42:26.086478 geojson_pydantic-1.1.0/.bumpversion.cfg
+-rw-r--r--   0        0        0     1173 2024-05-10 14:42:26.086478 geojson_pydantic-1.1.0/.gitignore
+-rw-r--r--   0        0        0      797 2024-05-10 14:42:26.086478 geojson_pydantic-1.1.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1073 2024-05-10 14:42:26.086478 geojson_pydantic-1.1.0/LICENSE
+-rw-r--r--   0        0        0     2892 2024-05-10 14:42:26.086478 geojson_pydantic-1.1.0/README.md
+-rw-r--r--   0        0        0      448 2024-05-10 14:42:26.090478 geojson_pydantic-1.1.0/geojson_pydantic/__init__.py
+-rw-r--r--   0        0        0     2925 2024-05-10 14:42:26.090478 geojson_pydantic-1.1.0/geojson_pydantic/base.py
+-rw-r--r--   0        0        0     1564 2024-05-10 14:42:26.090478 geojson_pydantic-1.1.0/geojson_pydantic/features.py
+-rw-r--r--   0        0        0    10662 2024-05-10 14:42:26.090478 geojson_pydantic-1.1.0/geojson_pydantic/geometries.py
+-rw-r--r--   0        0        0        0 2024-05-10 14:42:26.090478 geojson_pydantic-1.1.0/geojson_pydantic/py.typed
+-rw-r--r--   0        0        0      827 2024-05-10 14:42:26.090478 geojson_pydantic-1.1.0/geojson_pydantic/types.py
+-rw-r--r--   0        0        0     2254 2024-05-10 14:42:26.090478 geojson_pydantic-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     4053 1970-01-01 00:00:00.000000 geojson_pydantic-1.1.0/PKG-INFO
```

### Comparing `geojson_pydantic-1.0.2/.gitignore` & `geojson_pydantic-1.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `geojson_pydantic-1.0.2/.pre-commit-config.yaml` & `geojson_pydantic-1.1.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `geojson_pydantic-1.0.2/LICENSE` & `geojson_pydantic-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `geojson_pydantic-1.0.2/README.md` & `geojson_pydantic-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `geojson_pydantic-1.0.2/geojson_pydantic/base.py` & `geojson_pydantic-1.1.0/geojson_pydantic/base.py`

 * *Files identical despite different names*

### Comparing `geojson_pydantic-1.0.2/geojson_pydantic/features.py` & `geojson_pydantic-1.1.0/geojson_pydantic/features.py`

 * *Files identical despite different names*

### Comparing `geojson_pydantic-1.0.2/geojson_pydantic/geometries.py` & `geojson_pydantic-1.1.0/geojson_pydantic/geometries.py`

 * *Files identical despite different names*

### Comparing `geojson_pydantic-1.0.2/geojson_pydantic/types.py` & `geojson_pydantic-1.1.0/geojson_pydantic/types.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 """Types for geojson_pydantic models"""
 
-from typing import List, Tuple, Union
+from typing import List, NamedTuple, Tuple, Union
 
 from pydantic import Field
 from typing_extensions import Annotated
 
 BBox = Union[
     Tuple[float, float, float, float],  # 2D bbox
     Tuple[float, float, float, float, float, float],  # 3D bbox
 ]
 
-Position = Union[Tuple[float, float], Tuple[float, float, float]]
+Position2D = NamedTuple("Position2D", [("longitude", float), ("latitude", float)])
+Position3D = NamedTuple(
+    "Position3D", [("longitude", float), ("latitude", float), ("altitude", float)]
+)
+Position = Union[Position2D, Position3D]
 
 # Coordinate arrays
 LineStringCoords = Annotated[List[Position], Field(min_length=2)]
 LinearRing = Annotated[List[Position], Field(min_length=4)]
 MultiPointCoords = List[Position]
 MultiLineStringCoords = List[LineStringCoords]
 PolygonCoords = List[LinearRing]
```

### Comparing `geojson_pydantic-1.0.2/pyproject.toml` & `geojson_pydantic-1.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `geojson_pydantic-1.0.2/PKG-INFO` & `geojson_pydantic-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geojson-pydantic
-Version: 1.0.2
+Version: 1.1.0
 Summary: Pydantic data models for the GeoJSON spec.
 Keywords: geojson,Pydantic
 Author-email: Drew Bollinger <drew@developmentseed.org>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: geojson-pydantic Version: 1.0.2 Summary: Pydantic
+Metadata-Version: 2.1 Name: geojson-pydantic Version: 1.1.0 Summary: Pydantic
 data models for the GeoJSON spec. Keywords: geojson,Pydantic Author-email: Drew
 Bollinger
 developmentseed.org> Requires-Python: >=3.8 Description-Content-Type: text/
 markdown Classifier: Intended Audience :: Information Technology Classifier:
 Intended Audience :: Science/Research Classifier: License :: OSI Approved ::
 MIT License Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
```

