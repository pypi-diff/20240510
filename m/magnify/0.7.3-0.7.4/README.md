# Comparing `tmp/magnify-0.7.3.tar.gz` & `tmp/magnify-0.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "magnify-0.7.3.tar", max compression
+gzip compressed data, was "magnify-0.7.4.tar", max compression
```

## Comparing `magnify-0.7.3.tar` & `magnify-0.7.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     6937 2023-08-25 01:17:45.092814 magnify-0.7.3/README.md
--rw-r--r--   0        0        0     1637 2024-05-10 20:18:53.294165 magnify-0.7.3/pyproject.toml
--rw-r--r--   0        0        0      258 2024-05-10 20:18:37.717771 magnify-0.7.3/src/magnify/__init__.py
--rw-r--r--   0        0        0      675 2023-08-23 00:05:48.998305 magnify-0.7.3/src/magnify/accessor.py
--rw-r--r--   0        0        0      506 2023-08-22 23:14:29.137006 magnify-0.7.3/src/magnify/file.py
--rw-r--r--   0        0        0     3981 2023-12-07 00:53:02.766147 magnify-0.7.3/src/magnify/filter.py
--rw-r--r--   0        0        0    40698 2024-05-10 20:14:47.471988 magnify-0.7.3/src/magnify/find.py
--rw-r--r--   0        0        0     8625 2024-05-10 18:55:28.470792 magnify-0.7.3/src/magnify/identify.py
--rw-r--r--   0        0        0      880 2024-05-10 19:46:40.774434 magnify-0.7.3/src/magnify/logger.py
--rw-r--r--   0        0        0     3698 2024-05-10 19:01:10.012785 magnify-0.7.3/src/magnify/pipeline.py
--rw-r--r--   0        0        0      271 2023-08-22 18:49:02.746053 magnify-0.7.3/src/magnify/plot/__init__.py
--rw-r--r--   0        0        0     5218 2024-01-10 01:39:52.107079 magnify-0.7.3/src/magnify/plot/image.py
--rw-r--r--   0        0        0     3678 2023-08-24 23:52:07.029373 magnify-0.7.3/src/magnify/plot/ndplot.py
--rw-r--r--   0        0        0     1957 2023-11-22 02:51:21.867655 magnify-0.7.3/src/magnify/plot/relation.py
--rw-r--r--   0        0        0      154 2023-08-22 23:15:37.010790 magnify-0.7.3/src/magnify/plot/style.py
--rw-r--r--   0        0        0     1262 2024-01-10 01:58:38.923194 magnify-0.7.3/src/magnify/postprocess.py
--rw-r--r--   0        0        0     1380 2024-03-13 01:45:14.056154 magnify-0.7.3/src/magnify/preprocess.py
--rw-r--r--   0        0        0    15283 2024-05-10 18:42:38.572731 magnify-0.7.3/src/magnify/reader.py
--rw-r--r--   0        0        0     3418 2024-05-10 20:17:48.940540 magnify-0.7.3/src/magnify/registry.py
--rw-r--r--   0        0        0     1077 2023-12-07 00:52:30.105644 magnify-0.7.3/src/magnify/stitch.py
--rw-r--r--   0        0        0     2378 2024-01-10 02:01:55.479457 magnify-0.7.3/src/magnify/utils.py
--rw-r--r--   0        0        0     8159 1970-01-01 00:00:00.000000 magnify-0.7.3/PKG-INFO
+-rw-r--r--   0        0        0     6937 2023-08-25 01:17:45.092814 magnify-0.7.4/README.md
+-rw-r--r--   0        0        0     1637 2024-05-10 20:20:04.619970 magnify-0.7.4/pyproject.toml
+-rw-r--r--   0        0        0      258 2024-05-10 20:20:01.183883 magnify-0.7.4/src/magnify/__init__.py
+-rw-r--r--   0        0        0      675 2023-08-23 00:05:48.998305 magnify-0.7.4/src/magnify/accessor.py
+-rw-r--r--   0        0        0      506 2023-08-22 23:14:29.137006 magnify-0.7.4/src/magnify/file.py
+-rw-r--r--   0        0        0     3981 2023-12-07 00:53:02.766147 magnify-0.7.4/src/magnify/filter.py
+-rw-r--r--   0        0        0    40557 2024-05-10 20:19:40.559361 magnify-0.7.4/src/magnify/find.py
+-rw-r--r--   0        0        0     8625 2024-05-10 18:55:28.470792 magnify-0.7.4/src/magnify/identify.py
+-rw-r--r--   0        0        0      880 2024-05-10 19:46:40.774434 magnify-0.7.4/src/magnify/logger.py
+-rw-r--r--   0        0        0     3698 2024-05-10 19:01:10.012785 magnify-0.7.4/src/magnify/pipeline.py
+-rw-r--r--   0        0        0      271 2023-08-22 18:49:02.746053 magnify-0.7.4/src/magnify/plot/__init__.py
+-rw-r--r--   0        0        0     5218 2024-01-10 01:39:52.107079 magnify-0.7.4/src/magnify/plot/image.py
+-rw-r--r--   0        0        0     3678 2023-08-24 23:52:07.029373 magnify-0.7.4/src/magnify/plot/ndplot.py
+-rw-r--r--   0        0        0     1957 2023-11-22 02:51:21.867655 magnify-0.7.4/src/magnify/plot/relation.py
+-rw-r--r--   0        0        0      154 2023-08-22 23:15:37.010790 magnify-0.7.4/src/magnify/plot/style.py
+-rw-r--r--   0        0        0     1262 2024-01-10 01:58:38.923194 magnify-0.7.4/src/magnify/postprocess.py
+-rw-r--r--   0        0        0     1380 2024-03-13 01:45:14.056154 magnify-0.7.4/src/magnify/preprocess.py
+-rw-r--r--   0        0        0    15283 2024-05-10 18:42:38.572731 magnify-0.7.4/src/magnify/reader.py
+-rw-r--r--   0        0        0     3418 2024-05-10 20:17:48.940540 magnify-0.7.4/src/magnify/registry.py
+-rw-r--r--   0        0        0     1077 2023-12-07 00:52:30.105644 magnify-0.7.4/src/magnify/stitch.py
+-rw-r--r--   0        0        0     2378 2024-01-10 02:01:55.479457 magnify-0.7.4/src/magnify/utils.py
+-rw-r--r--   0        0        0     8159 1970-01-01 00:00:00.000000 magnify-0.7.4/PKG-INFO
```

### Comparing `magnify-0.7.3/README.md` & `magnify-0.7.4/README.md`

 * *Files identical despite different names*

### Comparing `magnify-0.7.3/pyproject.toml` & `magnify-0.7.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "magnify"
-version = "0.7.3"
+version = "0.7.4"
 description = "A microscopy image processing toolkit."
 authors = ["Karl Krauth <karl.krauth@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.8, <3.13"
 opencv-python = [
```

### Comparing `magnify-0.7.3/src/magnify/accessor.py` & `magnify-0.7.4/src/magnify/accessor.py`

 * *Files identical despite different names*

### Comparing `magnify-0.7.3/src/magnify/filter.py` & `magnify-0.7.4/src/magnify/filter.py`

 * *Files identical despite different names*

### Comparing `magnify-0.7.3/src/magnify/find.py` & `magnify-0.7.4/src/magnify/find.py`

 * *Files 1% similar despite different names*

```diff
@@ -210,17 +210,14 @@
                 grid_length=20,
                 num_iter=self.num_iter,
                 min_radius=self.min_button_radius,
                 max_radius=self.max_button_radius,
                 min_dist=min_button_dist,
                 min_roundness=self.min_roundness,
             )[:, :2]
-            import matplotlib.pyplot as plt
-            plt.imshow(image)
-            plt.scatter(new_points[:, 1], new_points[:, 0], c="r")
 
             if len(points) > 0:
                 # Remove points too close to other points in previous channels.
                 dist_matrix = np.linalg.norm(points[np.newaxis] - new_points[:, np.newaxis], axis=2)
                 new_points = new_points[np.min(dist_matrix, axis=1) > min_button_dist]
 
             # Add the new points to the list of seen points.
```

### Comparing `magnify-0.7.3/src/magnify/identify.py` & `magnify-0.7.4/src/magnify/identify.py`

 * *Files identical despite different names*

### Comparing `magnify-0.7.3/src/magnify/logger.py` & `magnify-0.7.4/src/magnify/logger.py`

 * *Files identical despite different names*

### Comparing `magnify-0.7.3/src/magnify/pipeline.py` & `magnify-0.7.4/src/magnify/pipeline.py`

 * *Files identical despite different names*

### Comparing `magnify-0.7.3/src/magnify/plot/image.py` & `magnify-0.7.4/src/magnify/plot/image.py`

 * *Files identical despite different names*

### Comparing `magnify-0.7.3/src/magnify/plot/ndplot.py` & `magnify-0.7.4/src/magnify/plot/ndplot.py`

 * *Files identical despite different names*

### Comparing `magnify-0.7.3/src/magnify/plot/relation.py` & `magnify-0.7.4/src/magnify/plot/relation.py`

 * *Files identical despite different names*

### Comparing `magnify-0.7.3/src/magnify/postprocess.py` & `magnify-0.7.4/src/magnify/postprocess.py`

 * *Files identical despite different names*

### Comparing `magnify-0.7.3/src/magnify/preprocess.py` & `magnify-0.7.4/src/magnify/preprocess.py`

 * *Files identical despite different names*

### Comparing `magnify-0.7.3/src/magnify/reader.py` & `magnify-0.7.4/src/magnify/reader.py`

 * *Files identical despite different names*

### Comparing `magnify-0.7.3/src/magnify/registry.py` & `magnify-0.7.4/src/magnify/registry.py`

 * *Files identical despite different names*

### Comparing `magnify-0.7.3/src/magnify/stitch.py` & `magnify-0.7.4/src/magnify/stitch.py`

 * *Files identical despite different names*

### Comparing `magnify-0.7.3/src/magnify/utils.py` & `magnify-0.7.4/src/magnify/utils.py`

 * *Files identical despite different names*

### Comparing `magnify-0.7.3/PKG-INFO` & `magnify-0.7.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: magnify
-Version: 0.7.3
+Version: 0.7.4
 Summary: A microscopy image processing toolkit.
 Author: Karl Krauth
 Author-email: karl.krauth@gmail.com
 Requires-Python: >=3.8,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

