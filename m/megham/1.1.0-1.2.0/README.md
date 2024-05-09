# Comparing `tmp/megham-1.1.0.tar.gz` & `tmp/megham-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "megham-1.1.0.tar", last modified: Tue Apr  2 23:47:15 2024, max compression
+gzip compressed data, was "megham-1.2.0.tar", last modified: Thu May  9 22:55:51 2024, max compression
```

## Comparing `megham-1.1.0.tar` & `megham-1.2.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 23:47:15.827749 megham-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-02 23:47:11.000000 megham-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4432 2024-04-02 23:47:15.827749 megham-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3630 2024-04-02 23:47:11.000000 megham-1.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 23:47:15.827749 megham-1.1.0/megham/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 23:47:11.000000 megham-1.1.0/megham/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14727 2024-04-02 23:47:11.000000 megham-1.1.0/megham/mds.py
--rw-r--r--   0 runner    (1001) docker     (127)    13565 2024-04-02 23:47:11.000000 megham-1.1.0/megham/transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     2588 2024-04-02 23:47:11.000000 megham-1.1.0/megham/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 23:47:15.827749 megham-1.1.0/megham.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4432 2024-04-02 23:47:15.000000 megham-1.1.0/megham.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-02 23:47:15.000000 megham-1.1.0/megham.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 23:47:15.000000 megham-1.1.0/megham.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-02 23:47:15.000000 megham-1.1.0/megham.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-02 23:47:15.000000 megham-1.1.0/megham.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      994 2024-04-02 23:47:11.000000 megham-1.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 23:47:15.827749 megham-1.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 22:55:51.154376 megham-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-09 22:55:47.000000 megham-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4432 2024-05-09 22:55:51.154376 megham-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3630 2024-05-09 22:55:47.000000 megham-1.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 22:55:51.154376 megham-1.2.0/megham/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 22:55:47.000000 megham-1.2.0/megham/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14727 2024-05-09 22:55:47.000000 megham-1.2.0/megham/mds.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15108 2024-05-09 22:55:47.000000 megham-1.2.0/megham/transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4173 2024-05-09 22:55:47.000000 megham-1.2.0/megham/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 22:55:51.154376 megham-1.2.0/megham.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4432 2024-05-09 22:55:51.000000 megham-1.2.0/megham.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-05-09 22:55:51.000000 megham-1.2.0/megham.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 22:55:51.000000 megham-1.2.0/megham.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-09 22:55:51.000000 megham-1.2.0/megham.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-09 22:55:51.000000 megham-1.2.0/megham.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      994 2024-05-09 22:55:47.000000 megham-1.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 22:55:51.154376 megham-1.2.0/setup.cfg
```

### Comparing `megham-1.1.0/LICENSE` & `megham-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `megham-1.1.0/PKG-INFO` & `megham-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: megham
-Version: 1.1.0
+Version: 1.2.0
 Summary: Tools for working with point clouds
 Author: Saianeesh Keshav Haridas
 License: GPLv3
 Keywords: point cloud,affine,rotations,mds,multidimensional scaling,point set registration,cpd,coherent point drift,mpd,guassian mixture model
 Classifier: Programming Language :: Python
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `megham-1.1.0/README.md` & `megham-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `megham-1.1.0/megham/mds.py` & `megham-1.2.0/megham/mds.py`

 * *Files identical despite different names*

### Comparing `megham-1.1.0/megham/transform.py` & `megham-1.2.0/megham/transform.py`

 * *Files 3% similar despite different names*

```diff
@@ -220,14 +220,57 @@
 
     transformed = src[msk] @ affine + shift
     shift += get_shift(transformed, dst[msk], **kwargs)
 
     return affine, shift
 
 
+def get_affine_two_stage(
+    src: NDArray[np.floating],
+    dst: NDArray[np.floating],
+    weights: NDArray[np.floating],
+) -> tuple[NDArray[np.floating], NDArray[np.floating]]:
+    """
+    Get affine transformation between two point clouds with a two stage solver.
+    This first uses the SVD to do an intitial alignment and
+    then uses weighted least squares to compute a correction on top of that.
+
+    Transformation is dst = affine@src + shift
+
+    Parameters
+    ----------
+    src : NDArray[np.floating]
+        A (npoints, ndim) array of source points.
+    dst : NDArray[np.floating]
+        A (npoints, ndim) array of destination points.
+    weights : NDArray[np.floating]
+        (npoints,) array of weights to use.
+        If provided a weighted least squares is done instead of an SVD.
+
+    Returns
+    -------
+    affine : NDArray[np.floating]
+        The (ndim, ndim) transformation matrix.
+    shift : NDArray[np.floating]
+        The (ndim,) shift to apply after transformation.
+    """
+    # Do an initial alignment without weights
+    affine_0, shift_0 = get_affine(src, dst, force_svd=True)
+    init_align = apply_transform(src, affine_0, shift_0)
+    # Now compute the actual transform
+    affine, shift = get_affine(init_align, dst, weights)
+    # Compose the transforms
+    affine, shift = compose_transform(affine_0, shift_0, affine, shift)
+    # Now one last shift correction
+    transformed = apply_transform(src, affine, shift)
+    shift += get_shift(transformed, dst, "mean", weights)
+
+    return affine, shift
+
+
 def apply_transform(
     src: NDArray[np.floating],
     transform: NDArray[np.floating],
     shift: NDArray[np.floating],
 ) -> NDArray[np.floating]:
     """
     Apply a transformation to a set of points.
```

### Comparing `megham-1.1.0/megham/utils.py` & `megham-1.2.0/megham/utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -66,23 +66,73 @@
     for dim_group in dim_groups:
         sq_diff = dist.cdist(src[:, dim_group], dst[:, dim_group], metric="sqeuclidean")
         var[dim_group] = np.nansum(sq_diff) / (len(dim_group) * nsrcpoints * ndstpoints)
 
     return var
 
 
-def estimate_spacing(coords: NDArray[np.floating]):
+def estimate_spacing(coords: NDArray[np.floating]) -> float:
     """
     Estimate the spacing between points in a point cloud.
     This is just the median distance between nearest neighbors.
 
     Parameters
     ----------
-    coords: NDArray[np.floating]
+    coords : NDArray[np.floating]
         The point cloud to estimate spacing of.
         Should have shape (npoint, ndim).
+
+    Returns
+    -------
+    spacing : float
+        The spacing between points.
     """
     edm = make_edm(coords)
     edm[edm == 0] = np.nan
     nearest_dists = np.nanmin(edm, axis=0)
 
     return np.median(nearest_dists)
+
+
+def gen_weights(
+    src: NDArray[np.floating],
+    dst: NDArray[np.floating],
+    var: Optional[NDArray[np.floating]] = None,
+    pdf: bool = False,
+) -> NDArray[np.floating]:
+    """
+    Generate weights between points in two registered point clouds.
+    The weight here is just the liklihood from a gaussian.
+    Note that this is not a GMM, each weight is computed from a single
+    gaussian since we are assuming a known registration.
+
+    Parameters
+    ----------
+    src : NDArray[np.floating]
+        The set of source points to be mapped onto the target points.
+        Should have shape (nsrcpoints, ndim).
+    dst : NDArray[np.floating]
+        The set of destination points to be mapped onto.
+        Should have shape (ndstpoints, ndim).
+    var : Optional[NDArray[np.floating]], default: None
+        The variance along each axis.
+        Should have shape (ndim,) if provided.
+        If None, will be computed with estimate_var
+    pdf : bool, default: False
+        If True apply the 1/sqrt(2*pi*var) normalization factor.
+        This makes the weights the PDF of a normal distribution.
+
+    Returns
+    -------
+    weights : NDArray[np.floating]
+        (npoints,) array of weights.
+    """
+    if var is None:
+        var = estimate_var(src, dst)
+    norm = np.ones_like(var)
+    if pdf:
+        norm = 1.0 / np.sqrt(2 * np.pi * var)
+
+    # Compute nd gaussian for each pair
+    weights = np.prod(norm * np.exp(-0.5 * (src - dst) ** 2 / var), axis=1)
+
+    return weights
```

### Comparing `megham-1.1.0/megham.egg-info/PKG-INFO` & `megham-1.2.0/megham.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: megham
-Version: 1.1.0
+Version: 1.2.0
 Summary: Tools for working with point clouds
 Author: Saianeesh Keshav Haridas
 License: GPLv3
 Keywords: point cloud,affine,rotations,mds,multidimensional scaling,point set registration,cpd,coherent point drift,mpd,guassian mixture model
 Classifier: Programming Language :: Python
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `megham-1.1.0/pyproject.toml` & `megham-1.2.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "megham"
-version = "1.1.0"
+version = "1.2.0"
 authors = [{name="Saianeesh Keshav Haridas"}]
 description = "Tools for working with point clouds"
 readme = "README.md"
 requires-python = ">=3.8"
 keywords = ["point cloud", "affine", "rotations", "mds", "multidimensional scaling", "point set registration", "cpd", "coherent point drift", "mpd", "guassian mixture model"]
 license = {text = "GPLv3"}
 classifiers = [ "Programming Language :: Python" ]
```

