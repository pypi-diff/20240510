# Comparing `tmp/invrs_opt-0.5.1.tar.gz` & `tmp/invrs_opt-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "invrs_opt-0.5.1.tar", last modified: Mon Apr  8 14:16:13 2024, max compression
+gzip compressed data, was "invrs_opt-0.5.2.tar", last modified: Fri May 10 15:53:02 2024, max compression
```

## Comparing `invrs_opt-0.5.1.tar` & `invrs_opt-0.5.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:16:13.872456 invrs_opt-0.5.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-04-08 14:16:01.000000 invrs_opt-0.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3318 2024-04-08 14:16:13.872456 invrs_opt-0.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-04-08 14:16:01.000000 invrs_opt-0.5.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-04-08 14:16:01.000000 invrs_opt-0.5.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 14:16:13.872456 invrs_opt-0.5.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:16:13.868456 invrs_opt-0.5.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:16:13.868456 invrs_opt-0.5.1/src/invrs_opt/
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-08 14:16:01.000000 invrs_opt-0.5.1/src/invrs_opt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      907 2024-04-08 14:16:01.000000 invrs_opt-0.5.1/src/invrs_opt/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:16:13.872456 invrs_opt-0.5.1/src/invrs_opt/experimental/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 14:16:01.000000 invrs_opt-0.5.1/src/invrs_opt/experimental/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4842 2024-04-08 14:16:01.000000 invrs_opt-0.5.1/src/invrs_opt/experimental/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      562 2024-04-08 14:16:01.000000 invrs_opt-0.5.1/src/invrs_opt/experimental/labels.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:16:13.872456 invrs_opt-0.5.1/src/invrs_opt/lbfgsb/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 14:16:01.000000 invrs_opt-0.5.1/src/invrs_opt/lbfgsb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27892 2024-04-08 14:16:01.000000 invrs_opt-0.5.1/src/invrs_opt/lbfgsb/lbfgsb.py
--rw-r--r--   0 runner    (1001) docker     (127)     5971 2024-04-08 14:16:01.000000 invrs_opt-0.5.1/src/invrs_opt/lbfgsb/transform.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 14:16:01.000000 invrs_opt-0.5.1/src/invrs_opt/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:16:13.872456 invrs_opt-0.5.1/src/invrs_opt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3318 2024-04-08 14:16:13.000000 invrs_opt-0.5.1/src/invrs_opt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      518 2024-04-08 14:16:13.000000 invrs_opt-0.5.1/src/invrs_opt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 14:16:13.000000 invrs_opt-0.5.1/src/invrs_opt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-08 14:16:13.000000 invrs_opt-0.5.1/src/invrs_opt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-08 14:16:13.000000 invrs_opt-0.5.1/src/invrs_opt.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:16:13.872456 invrs_opt-0.5.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     8991 2024-04-08 14:16:01.000000 invrs_opt-0.5.1/tests/test_algos.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:53:02.796263 invrs_opt-0.5.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-05-10 15:52:52.000000 invrs_opt-0.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3318 2024-05-10 15:53:02.796263 invrs_opt-0.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-05-10 15:52:52.000000 invrs_opt-0.5.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-05-10 15:52:52.000000 invrs_opt-0.5.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 15:53:02.796263 invrs_opt-0.5.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:53:02.788263 invrs_opt-0.5.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:53:02.792263 invrs_opt-0.5.2/src/invrs_opt/
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-10 15:52:52.000000 invrs_opt-0.5.2/src/invrs_opt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      907 2024-05-10 15:52:52.000000 invrs_opt-0.5.2/src/invrs_opt/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:53:02.792263 invrs_opt-0.5.2/src/invrs_opt/experimental/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 15:52:52.000000 invrs_opt-0.5.2/src/invrs_opt/experimental/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4842 2024-05-10 15:52:52.000000 invrs_opt-0.5.2/src/invrs_opt/experimental/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      562 2024-05-10 15:52:52.000000 invrs_opt-0.5.2/src/invrs_opt/experimental/labels.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:53:02.792263 invrs_opt-0.5.2/src/invrs_opt/lbfgsb/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 15:52:52.000000 invrs_opt-0.5.2/src/invrs_opt/lbfgsb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27820 2024-05-10 15:52:52.000000 invrs_opt-0.5.2/src/invrs_opt/lbfgsb/lbfgsb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5971 2024-05-10 15:52:52.000000 invrs_opt-0.5.2/src/invrs_opt/lbfgsb/transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 15:52:52.000000 invrs_opt-0.5.2/src/invrs_opt/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:53:02.792263 invrs_opt-0.5.2/src/invrs_opt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3318 2024-05-10 15:53:02.000000 invrs_opt-0.5.2/src/invrs_opt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      518 2024-05-10 15:53:02.000000 invrs_opt-0.5.2/src/invrs_opt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 15:53:02.000000 invrs_opt-0.5.2/src/invrs_opt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-10 15:53:02.000000 invrs_opt-0.5.2/src/invrs_opt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-10 15:53:02.000000 invrs_opt-0.5.2/src/invrs_opt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:53:02.792263 invrs_opt-0.5.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     8991 2024-05-10 15:52:52.000000 invrs_opt-0.5.2/tests/test_algos.py
```

### Comparing `invrs_opt-0.5.1/LICENSE` & `invrs_opt-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `invrs_opt-0.5.1/PKG-INFO` & `invrs_opt-0.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invrs_opt
-Version: 0.5.1
+Version: 0.5.2
 Summary: Algorithms for inverse design
 Author-email: "Martin F. Schubert" <mfschubert@gmail.com>
 Maintainer-email: "Martin F. Schubert" <mfschubert@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 The INVRS-IO authors.
         
@@ -45,15 +45,15 @@
 Provides-Extra: dev
 Requires-Dist: bump-my-version; extra == "dev"
 Requires-Dist: darglint; extra == "dev"
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 
 # invrs-opt - Optimization algorithms for inverse design
-`v0.5.1`
+`v0.5.2`
 
 ## Overview
 
 The `invrs-opt` package defines an optimizer API intended for topology optimization, inverse design, or AI-guided design. It (currently) implements the L-BFGS-B optimization algorithm along with some variants. The API is intended to be general so that new algorithms can be accommodated, and is inspired by the functional optimizer approach used in jax. Example usage is as follows:
 
 ```python
 initial_params = ...
```

### Comparing `invrs_opt-0.5.1/README.md` & `invrs_opt-0.5.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # invrs-opt - Optimization algorithms for inverse design
-`v0.5.1`
+`v0.5.2`
 
 ## Overview
 
 The `invrs-opt` package defines an optimizer API intended for topology optimization, inverse design, or AI-guided design. It (currently) implements the L-BFGS-B optimization algorithm along with some variants. The API is intended to be general so that new algorithms can be accommodated, and is inspired by the functional optimizer approach used in jax. Example usage is as follows:
 
 ```python
 initial_params = ...
```

### Comparing `invrs_opt-0.5.1/pyproject.toml` & `invrs_opt-0.5.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 
 name = "invrs_opt"
-version = "v0.5.1"
+version = "v0.5.2"
 description = "Algorithms for inverse design"
 keywords = ["topology", "optimization", "jax", "inverse design"]
 readme = "README.md"
 requires-python = ">=3.7"
 license = {file = "LICENSE"}
 
 authors = [
```

### Comparing `invrs_opt-0.5.1/src/invrs_opt/base.py` & `invrs_opt-0.5.2/src/invrs_opt/base.py`

 * *Files identical despite different names*

### Comparing `invrs_opt-0.5.1/src/invrs_opt/experimental/client.py` & `invrs_opt-0.5.2/src/invrs_opt/experimental/client.py`

 * *Files identical despite different names*

### Comparing `invrs_opt-0.5.1/src/invrs_opt/experimental/labels.py` & `invrs_opt-0.5.2/src/invrs_opt/experimental/labels.py`

 * *Files identical despite different names*

### Comparing `invrs_opt-0.5.1/src/invrs_opt/lbfgsb/lbfgsb.py` & `invrs_opt-0.5.2/src/invrs_opt/lbfgsb/lbfgsb.py`

 * *Files 1% similar despite different names*

```diff
@@ -254,15 +254,15 @@
             )
             latent_params = _to_pytree(scipy_lbfgsb_state.x, params)
             return latent_params, scipy_lbfgsb_state.to_jax()
 
         (
             latent_params,
             jax_lbfgsb_state,
-        ) = jax.pure_callback(  # type: ignore[attr-defined]
+        ) = jax.pure_callback(
             _init_pure,
             _example_state(params, maxcor),
             initialize_latent_fn(params),
         )
         return transform_fn(latent_params), latent_params, jax_lbfgsb_state
 
     def params_fn(state: LbfgsbState) -> PyTree:
@@ -300,15 +300,15 @@
         flat_latent_grad, unflatten_fn = flatten_util.ravel_pytree(
             latent_grad
         )  # type: ignore[no-untyped-call]
 
         (
             flat_latent_params,
             jax_lbfgsb_state,
-        ) = jax.pure_callback(  # type: ignore[attr-defined]
+        ) = jax.pure_callback(
             _update_pure,
             (flat_latent_grad, jax_lbfgsb_state),
             flat_latent_grad,
             value,
             jax_lbfgsb_state,
         )
         latent_params = unflatten_fn(flat_latent_params)
@@ -538,27 +538,27 @@
         )
 
     @classmethod
     def from_jax(cls, state_dict: Dict[str, jnp.ndarray]) -> "ScipyLbfgsbState":
         """Converts a dictionary of jax arrays to a `ScipyLbfgsbState`."""
         state_dict = copy.deepcopy(state_dict)
         return ScipyLbfgsbState(
-            x=onp.asarray(state_dict["x"], dtype=onp.float64),
+            x=onp.array(state_dict["x"], dtype=onp.float64),
             converged=onp.asarray(state_dict["converged"], dtype=bool),
             _maxcor=int(state_dict["_maxcor"]),
             _line_search_max_steps=int(state_dict["_line_search_max_steps"]),
             _ftol=onp.asarray(state_dict["_ftol"], dtype=onp.float64),
             _gtol=onp.asarray(state_dict["_gtol"], dtype=onp.float64),
-            _wa=onp.asarray(state_dict["_wa"], onp.float64),
-            _iwa=onp.asarray(state_dict["_iwa"], dtype=FORTRAN_INT),
+            _wa=onp.array(state_dict["_wa"], onp.float64),
+            _iwa=onp.array(state_dict["_iwa"], dtype=FORTRAN_INT),
             _task=_s60_str_from_array(state_dict["_task"]),
             _csave=_s60_str_from_array(state_dict["_csave"]),
-            _lsave=onp.asarray(state_dict["_lsave"], dtype=FORTRAN_INT),
-            _isave=onp.asarray(state_dict["_isave"], dtype=FORTRAN_INT),
-            _dsave=onp.asarray(state_dict["_dsave"], dtype=onp.float64),
+            _lsave=onp.array(state_dict["_lsave"], dtype=FORTRAN_INT),
+            _isave=onp.array(state_dict["_isave"], dtype=FORTRAN_INT),
+            _dsave=onp.array(state_dict["_dsave"], dtype=onp.float64),
             _lower_bound=onp.asarray(state_dict["_lower_bound"], dtype=onp.float64),
             _upper_bound=onp.asarray(state_dict["_upper_bound"], dtype=onp.float64),
             _bound_type=onp.asarray(state_dict["_bound_type"], dtype=int),
         )
 
     @classmethod
     def init(
```

### Comparing `invrs_opt-0.5.1/src/invrs_opt/lbfgsb/transform.py` & `invrs_opt-0.5.2/src/invrs_opt/lbfgsb/transform.py`

 * *Files identical despite different names*

### Comparing `invrs_opt-0.5.1/src/invrs_opt.egg-info/PKG-INFO` & `invrs_opt-0.5.2/src/invrs_opt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invrs_opt
-Version: 0.5.1
+Version: 0.5.2
 Summary: Algorithms for inverse design
 Author-email: "Martin F. Schubert" <mfschubert@gmail.com>
 Maintainer-email: "Martin F. Schubert" <mfschubert@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 The INVRS-IO authors.
         
@@ -45,15 +45,15 @@
 Provides-Extra: dev
 Requires-Dist: bump-my-version; extra == "dev"
 Requires-Dist: darglint; extra == "dev"
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 
 # invrs-opt - Optimization algorithms for inverse design
-`v0.5.1`
+`v0.5.2`
 
 ## Overview
 
 The `invrs-opt` package defines an optimizer API intended for topology optimization, inverse design, or AI-guided design. It (currently) implements the L-BFGS-B optimization algorithm along with some variants. The API is intended to be general so that new algorithms can be accommodated, and is inspired by the functional optimizer approach used in jax. Example usage is as follows:
 
 ```python
 initial_params = ...
```

### Comparing `invrs_opt-0.5.1/src/invrs_opt.egg-info/SOURCES.txt` & `invrs_opt-0.5.2/src/invrs_opt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `invrs_opt-0.5.1/tests/test_algos.py` & `invrs_opt-0.5.2/tests/test_algos.py`

 * *Files identical despite different names*

