# Comparing `tmp/nutils_poly-1.0.0.tar.gz` & `tmp/nutils_poly-1.0.1.tar.gz`

## Comparing `nutils_poly-1.0.0.tar` & `nutils_poly-1.0.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      526 1970-01-01 00:00:00.000000 nutils_poly-1.0.0/Cargo.toml
--rw-r--r--   0     1001      123       13 2023-01-18 11:13:20.000000 nutils_poly-1.0.0/.codecov.yml
--rw-r--r--   0     1001      123      811 2023-01-18 11:13:20.000000 nutils_poly-1.0.0/.github/workflows/ci.yaml
--rw-r--r--   0     1001      123       21 2023-01-18 11:13:20.000000 nutils_poly-1.0.0/.gitignore
--rw-r--r--   0     1001      123     1329 2023-01-18 11:13:20.000000 nutils_poly-1.0.0/README.md
--rw-r--r--   0     1001      123      666 2023-01-18 11:13:20.000000 nutils_poly-1.0.0/docs/conf.py
--rw-r--r--   0     1001      123       66 2023-01-18 11:13:20.000000 nutils_poly-1.0.0/docs/index.rst
--rw-r--r--   0     1001      123      416 2023-01-18 11:13:20.000000 nutils_poly-1.0.0/pyproject.toml
--rw-r--r--   0     1001      123    41783 2023-01-18 11:13:20.000000 nutils_poly-1.0.0/src/lib.rs
--rw-r--r--   0     1001      123    11554 2023-01-18 11:13:20.000000 nutils_poly-1.0.0/test.py
--rw-r--r--   0     1001      123    12192 2023-01-18 11:13:20.000000 nutils_poly-1.0.0/Cargo.lock
--rw-r--r--   0        0        0     1911 1970-01-01 00:00:00.000000 nutils_poly-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      526 1970-01-01 00:00:00.000000 nutils_poly-1.0.1/Cargo.toml
+-rw-r--r--   0     1001      127       13 2024-05-08 20:25:09.000000 nutils_poly-1.0.1/.codecov.yml
+-rw-r--r--   0     1001      127      810 2024-05-08 20:25:09.000000 nutils_poly-1.0.1/.github/workflows/ci.yaml
+-rw-r--r--   0     1001      127       21 2024-05-08 20:25:09.000000 nutils_poly-1.0.1/.gitignore
+-rw-r--r--   0     1001      127     1329 2024-05-08 20:25:09.000000 nutils_poly-1.0.1/README.md
+-rw-r--r--   0     1001      127      666 2024-05-08 20:25:09.000000 nutils_poly-1.0.1/docs/conf.py
+-rw-r--r--   0     1001      127       66 2024-05-08 20:25:09.000000 nutils_poly-1.0.1/docs/index.rst
+-rw-r--r--   0     1001      127    41981 2024-05-08 20:25:09.000000 nutils_poly-1.0.1/src/lib.rs
+-rw-r--r--   0     1001      127    11554 2024-05-08 20:25:09.000000 nutils_poly-1.0.1/test.py
+-rw-r--r--   0     1001      127    12362 2024-05-08 20:25:09.000000 nutils_poly-1.0.1/Cargo.lock
+-rw-r--r--   0     1001      127      414 2024-05-08 20:25:09.000000 nutils_poly-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     1911 1970-01-01 00:00:00.000000 nutils_poly-1.0.1/PKG-INFO
```

### Comparing `nutils_poly-1.0.0/Cargo.toml` & `nutils_poly-1.0.1/Cargo.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [package]
 name = "nutils-poly-py"
-version = "1.0.0"
+version = "1.0.1"
 authors = ["Evalf <info@evalf.com>"]
 edition = "2021"
 license = "MIT"
 repository = "https://github.com/nutils/poly-py"
 description = "Low-level functions for evaluating and manipulating polynomials (Python bindings)"
 
 [lib]
 name = "nutils_poly"
 crate-type = ["cdylib"]
 
 [dependencies]
 ndarray = "0.15"
-numpy = "0.17"
+numpy = "0.21"
 nutils-poly = "1"
-pyo3 = { version = "0.17", features = ["extension-module", "abi3-py37"] }
+pyo3 = { version = "0.21", features = ["extension-module", "abi3-py38"] }
 sha1 = "0.10.5"
 sqnc = { version = "1", features = ["ndarray"] }
```

### Comparing `nutils_poly-1.0.0/.github/workflows/ci.yaml` & `nutils_poly-1.0.1/.github/workflows/ci.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -9,16 +9,16 @@
   package:
     name: Build and test package
     uses: evalf/workflow-maturin/.github/workflows/build-and-test.yaml@release/1
     with:
       targets: |
         defaults = dict(python='cp310', test=True)
         targets = []
-        targets.extend(defaults | dict(os='linux', arch=arch) for arch in ('x86_64', 'aarch64'))
-        targets.extend(defaults | dict(os='macos', arch=arch) for arch in ('x86_64', 'universal2'))
+        targets.extend(defaults | dict(os=os, arch=arch) for os in ('linux', 'musllinux') for arch in ('x86_64', 'aarch64'))
+        targets.append(defaults | dict(os='macos', arch='universal2'))
         targets.extend(defaults | dict(os='windows', arch=arch) for arch in ('x86_64', 'i686'))
   docs:
     name: Build documentation
     needs: package
     uses: evalf/workflow-sphinx/.github/workflows/build.yaml@release/1
     with:
       # tomli is needed for Python<3.11
```

### Comparing `nutils_poly-1.0.0/README.md` & `nutils_poly-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `nutils_poly-1.0.0/docs/conf.py` & `nutils_poly-1.0.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `nutils_poly-1.0.0/src/lib.rs` & `nutils_poly-1.0.1/src/lib.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 use ndarray::{ArrayBase, ArrayD, ArrayViewD, Data, Dimension};
-use numpy::{PyArray, PyArray2, PyArrayDyn, PyReadonlyArray2, PyReadonlyArrayDyn, ToPyArray};
+use numpy::{
+    PyArray, PyArray2, PyArrayDyn, PyArrayMethods, PyReadonlyArray2, PyReadonlyArrayDyn,
+    PyUntypedArrayMethods, ToPyArray,
+};
 use nutils_poly::{MulPlan, MulVar, PartialDerivPlan, Power};
 use pyo3::class::basic::CompareOp;
 use pyo3::exceptions::PyValueError;
 use pyo3::prelude::*;
 use pyo3::types::PyBytes;
 use sha1::{Digest, Sha1};
 use sqnc::traits::*;
@@ -215,15 +218,15 @@
 /// :func:`eval_outer` : Evaluates all pairs of coefficients and values.
 #[pyfunction]
 #[pyo3(text_signature = "(coeffs, coords)")]
 fn eval<'py>(
     py: Python<'py>,
     coeffs: PyReadonlyArrayDyn<f64>,
     values: PyReadonlyArrayDyn<f64>,
-) -> PyResult<&'py PyArrayDyn<f64>> {
+) -> PyResult<Bound<'py, PyArrayDyn<f64>>> {
     let values = values.as_array();
     let Some((nvars, values_leading_shape)) = values.shape().split_last() else {
         return Err(PyValueError::new_err("expected `values` with at least one axis"));
     };
     let (coeffs, degree, ncoeffs, coeffs_leading_shape) = as_coeffs_dyn(&coeffs, *nvars, "coeffs")?;
     let result_shape = broadcast_shapes(&[coeffs_leading_shape, values_leading_shape])?;
     let coeffs = coeffs.broadcast(shape![&result_shape, [ncoeffs]]).unwrap();
@@ -241,15 +244,15 @@
             );
         }
     } else {
         for (coeffs, values) in iter::zip(coeffs.rows(), values.rows()) {
             result.push(nutils_poly::eval(coeffs, &values, degree).unwrap());
         }
     }
-    PyArray::from_vec(py, result).reshape(result_shape)
+    PyArray::from_vec_bound(py, result).reshape(result_shape)
 }
 
 /// Evaluates all pairs of polynomials and values.
 ///
 /// The degree of the polynomial and the number of variables are automatically
 /// determined from the lengths of the last axes of the arguments.
 ///
@@ -272,15 +275,15 @@
 /// :func:`eval` : Evaluates joined polynomials and values.
 #[pyfunction]
 #[pyo3(text_signature = "(coeffs, coords)")]
 fn eval_outer<'py>(
     py: Python<'py>,
     coeffs: PyReadonlyArrayDyn<f64>,
     values: PyReadonlyArrayDyn<f64>,
-) -> PyResult<&'py PyArrayDyn<f64>> {
+) -> PyResult<Bound<'py, PyArrayDyn<f64>>> {
     let values = values.as_array();
     let Some((nvars, values_leading_shape)) = values.shape().split_last() else {
         return Err(PyValueError::new_err("expected `values` with at least one axis"));
     };
     let (coeffs, degree, _, coeffs_leading_shape) = as_coeffs_dyn(&coeffs, *nvars, "coeffs")?;
     let result_shape = shape![values_leading_shape, coeffs_leading_shape];
     let mut result = Vec::with_capacity(result_shape.iter().copied().product());
@@ -314,15 +317,15 @@
         for values in values.rows() {
             contig_values.assign(values.copied().iter()).unwrap();
             for coeffs in coeffs.rows() {
                 result.push(nutils_poly::eval(coeffs, &contig_values, degree).unwrap());
             }
         }
     }
-    PyArray::from_vec(py, result).reshape(result_shape)
+    PyArray::from_vec_bound(py, result).reshape(result_shape)
 }
 
 /// Plan for the partial derivative of a polynomial.
 ///
 /// The plan can be applied to coefficients (``plan(coeffs)``) to obtain the
 /// coefficients for the partial derivative of the polynomial.
 ///
@@ -349,49 +352,49 @@
 /// ... )
 ///
 /// See also
 /// --------
 /// :func:`partial_deriv` : Compute the partial derivative without a plan.
 /// :func:`GradPlan` : Plan for the gradient of a polynomial.
 #[pyclass]
-#[pyo3(name = "PartialDerivPlan")]
+#[pyo3(name = "PartialDerivPlan", module = "nutils_poly")]
 #[derive(Debug, Clone)]
-#[pyo3(text_signature = "(nvars, degree, var)", module = "nutils_poly")]
 struct PyPartialDerivPlan(PartialDerivPlan);
 
 #[pymethods]
 impl PyPartialDerivPlan {
     #[new]
+    #[pyo3(text_signature = "(nvars, degree, var)")]
     fn new(nvars: usize, degree: Power, var: usize) -> PyResult<Self> {
         if let Some(plan) = PartialDerivPlan::new(nvars, degree, var) {
             Ok(Self(plan))
         } else {
             Err(PyValueError::new_err(format!("the (index of the) variable to plan the partial derivative for ({var}) exceeds the number of variables ({nvars})")))
         }
     }
     fn __call__<'py>(
         &self,
         py: Python<'py>,
         coeffs: PyReadonlyArrayDyn<f64>,
-    ) -> PyResult<&'py PyArrayDyn<f64>> {
+    ) -> PyResult<Bound<'py, PyArrayDyn<f64>>> {
         let (coeffs, leading_shape) =
             as_coeffs_dyn_with_ncoeffs(&coeffs, self.0.ncoeffs_input(), "coeffs")?;
         let result_shape = shape![leading_shape, [self.0.ncoeffs_output()]];
         let mut result = Vec::with_capacity(result_shape.iter().copied().product());
         if has_contiguous_rows(&coeffs) {
             for coeffs in coeffs.rows() {
                 let coeffs = coeffs.as_slice().unwrap().as_sqnc();
                 result.extend(self.0.apply(coeffs).unwrap().iter());
             }
         } else {
             for coeffs in coeffs.rows() {
                 result.extend(self.0.apply(coeffs).unwrap().iter());
             }
         }
-        PyArray::from_vec(py, result).reshape(result_shape)
+        PyArray::from_vec_bound(py, result).reshape(result_shape)
     }
 }
 
 /// Returns the coefficients for the partial derivative of a polynomial.
 ///
 /// Args
 /// ----
@@ -436,15 +439,15 @@
 #[pyfunction]
 #[pyo3(text_signature = "(coeffs, nvars)")]
 fn partial_deriv<'py>(
     py: Python<'py>,
     coeffs: PyReadonlyArrayDyn<f64>,
     nvars: usize,
     var: usize,
-) -> PyResult<&'py PyArrayDyn<f64>> {
+) -> PyResult<Bound<'py, PyArrayDyn<f64>>> {
     let Some(ncoeffs) = coeffs.shape().last() else {
         return Err(PyValueError::new_err("expected `coeffs` with at least one axis"));
     };
     let degree = degree(nvars, *ncoeffs)?;
     PyPartialDerivPlan::new(nvars, degree, var)?.__call__(py, coeffs)
 }
 
@@ -461,26 +464,26 @@
 ///     The degree of the polynomial.
 ///
 /// See also
 /// --------
 /// :func:`grad` : Compute the gradient without a plan.
 /// :func:`PartialDerivPlan` : Plan for the partial derivative of a polynomial.
 #[pyclass]
-#[pyo3(name = "GradPlan")]
+#[pyo3(name = "GradPlan", module = "nutils_poly")]
 #[derive(Debug, Clone)]
-#[pyo3(text_signature = "(nvars, degree)", module = "nutils_poly")]
 struct PyGradPlan {
     plans: Box<[PartialDerivPlan]>,
     ncoeffs_input: usize,
     ncoeffs_output: usize,
 }
 
 #[pymethods]
 impl PyGradPlan {
     #[new]
+    #[pyo3(text_signature = "(nvars, degree)")]
     fn new(nvars: usize, degree: Power) -> Self {
         let plans: Box<[_]> = Iterator::map(0..nvars, |var| {
             PartialDerivPlan::new(nvars, degree, var).unwrap()
         })
         .collect();
         let (ncoeffs_input, ncoeffs_output) = if let Some(plan) = plans.first() {
             (plan.ncoeffs_input(), plan.ncoeffs_output())
@@ -493,15 +496,15 @@
             ncoeffs_output,
         }
     }
     fn __call__<'py>(
         &self,
         py: Python<'py>,
         coeffs: PyReadonlyArrayDyn<f64>,
-    ) -> PyResult<&'py PyArrayDyn<f64>> {
+    ) -> PyResult<Bound<'py, PyArrayDyn<f64>>> {
         let (coeffs, leading_shape) =
             as_coeffs_dyn_with_ncoeffs(&coeffs, self.ncoeffs_input, "coeffs")?;
         let result_shape = shape![leading_shape, [self.plans.len(), self.ncoeffs_output]];
         let mut result = Vec::with_capacity(result_shape.iter().copied().product());
         if has_contiguous_rows(&coeffs) {
             for coeffs in coeffs.rows() {
                 for plan in self.plans.iter() {
@@ -512,15 +515,15 @@
         } else {
             for coeffs in coeffs.rows() {
                 for plan in self.plans.iter() {
                     result.extend(plan.apply(coeffs).unwrap().iter());
                 }
             }
         }
-        PyArray::from_vec(py, result).reshape(result_shape)
+        PyArray::from_vec_bound(py, result).reshape(result_shape)
     }
     #[getter]
     fn ncoeffs_output(&self) -> usize {
         self.ncoeffs_output
     }
 }
 
@@ -555,15 +558,15 @@
 /// :func:`partial_deriv` : Compute the partial derivative of a polynomial.
 #[pyfunction]
 #[pyo3(text_signature = "(coeffs, nvars)")]
 fn grad<'py>(
     py: Python<'py>,
     coeffs: PyReadonlyArrayDyn<f64>,
     nvars: usize,
-) -> PyResult<&'py PyArrayDyn<f64>> {
+) -> PyResult<Bound<'py, PyArrayDyn<f64>>> {
     let Some(ncoeffs) = coeffs.shape().last() else {
         return Err(PyValueError::new_err("expected `coeffs` with at least one axis"));
     };
     let degree = degree(nvars, *ncoeffs)?;
     PyGradPlan::new(nvars, degree).__call__(py, coeffs)
 }
 
@@ -630,19 +633,19 @@
     }
     fn __hash__(&self) -> u64 {
         let mut hasher = DefaultHasher::new();
         self.0.hash(&mut hasher);
         hasher.finish()
     }
     #[getter]
-    fn __nutils_hash__<'py>(&self, py: Python<'py>) -> &'py PyBytes {
+    fn __nutils_hash__<'py>(&self, py: Python<'py>) -> Bound<'py, PyBytes> {
         let mut hasher = Sha1::new();
         hasher.update(self.__repr__().as_bytes());
         let digest = hasher.finalize();
-        PyBytes::new(py, &digest)
+        PyBytes::new_bound(py, &digest)
     }
 }
 
 /// Plan for the product of two polynomials.
 ///
 /// The plan can be applied to a pair of coefficients (``plan(coeffs_left,
 /// coeffs_right, vars)``) to obtain the coefficients for the product of
@@ -686,25 +689,22 @@
 ///
 /// See also
 /// --------
 /// :func:`mul` : Compute the multiplication without a plan.
 /// :meth:`MulPlan.same_vars` : Create a plan for the multiplication of two polynomials in the same variables.
 /// :meth:`MulPlan.different_vars` : Create a plan for the multiplication of two polynomials in different variables.
 #[pyclass]
-#[pyo3(name = "MulPlan")]
-#[pyo3(
-    text_signature = "(vars, degree_left, degree_right)",
-    module = "nutils_poly"
-)]
+#[pyo3(name = "MulPlan", module = "nutils_poly")]
 #[derive(Debug, Clone)]
 struct PyMulPlan(MulPlan);
 
 #[pymethods]
 impl PyMulPlan {
     #[new]
+    #[pyo3(text_signature = "(vars, degree_left, degree_right)")]
     fn new(vars: Vec<PyMulVar>, degree_left: Power, degree_right: Power) -> Self {
         Self(MulPlan::new(
             &vars.as_sqnc().map(|var| var.0),
             degree_left,
             degree_right,
         ))
     }
@@ -747,15 +747,15 @@
         ))
     }
     fn __call__<'py>(
         &self,
         py: Python<'py>,
         coeffs_left: PyReadonlyArrayDyn<f64>,
         coeffs_right: PyReadonlyArrayDyn<f64>,
-    ) -> PyResult<&'py PyArrayDyn<f64>> {
+    ) -> PyResult<Bound<'py, PyArrayDyn<f64>>> {
         let (coeffs_left, leading_shape_left) =
             as_coeffs_dyn_with_ncoeffs(&coeffs_left, self.0.ncoeffs_left(), "coeffs_left")?;
         let (coeffs_right, leading_shape_right) =
             as_coeffs_dyn_with_ncoeffs(&coeffs_right, self.0.ncoeffs_right(), "coeffs_right")?;
         let leading_shape = broadcast_shapes(&[leading_shape_left, leading_shape_right])?;
         let coeffs_left = coeffs_left
             .broadcast(shape![&leading_shape, [self.0.ncoeffs_left()]])
@@ -772,15 +772,15 @@
                 result.extend(self.0.apply(coeffs_left, coeffs_right).unwrap().iter());
             }
         } else {
             for (coeffs_left, coeffs_right) in iter::zip(coeffs_left.rows(), coeffs_right.rows()) {
                 result.extend(self.0.apply(coeffs_left, coeffs_right).unwrap().iter());
             }
         }
-        PyArray::from_vec(py, result).reshape(result_shape)
+        PyArray::from_vec_bound(py, result).reshape(result_shape)
     }
     #[getter]
     fn ncoeffs_output(&self) -> usize {
         self.0.ncoeffs_output()
     }
 }
 
@@ -849,15 +849,15 @@
 #[pyfunction]
 #[pyo3(text_signature = "(coeffs_left, coeffs_right, vars)")]
 fn mul<'py>(
     py: Python<'py>,
     coeffs_left: PyReadonlyArrayDyn<f64>,
     coeffs_right: PyReadonlyArrayDyn<f64>,
     vars: Vec<PyMulVar>,
-) -> PyResult<&'py PyArrayDyn<f64>> {
+) -> PyResult<Bound<'py, PyArrayDyn<f64>>> {
     let Some(ncoeffs_left) = coeffs_left.shape().last() else {
         return Err(PyValueError::new_err("expected `coeffs_left` with at least one axis"));
     };
     let Some(ncoeffs_right) = coeffs_right.shape().last() else {
         return Err(PyValueError::new_err("expected `coeffs_right` with at least one axis"));
     };
     let nvars_left = vars.iter().filter(|var| var.0 != MulVar::Right).count();
@@ -919,15 +919,15 @@
 #[pyfunction]
 #[pyo3(text_signature = "(coeffs_left, coeffs_right, nvars)")]
 fn mul_same_vars<'py>(
     py: Python<'py>,
     coeffs_left: PyReadonlyArrayDyn<f64>,
     coeffs_right: PyReadonlyArrayDyn<f64>,
     nvars: usize,
-) -> PyResult<&'py PyArrayDyn<f64>> {
+) -> PyResult<Bound<'py, PyArrayDyn<f64>>> {
     let Some(ncoeffs_left) = coeffs_left.shape().last() else {
         return Err(PyValueError::new_err("expected `coeffs_left` with at least one axis"));
     };
     let Some(ncoeffs_right) = coeffs_right.shape().last() else {
         return Err(PyValueError::new_err("expected `coeffs_right` with at least one axis"));
     };
     let degree_left = degree(nvars, *ncoeffs_left)?;
@@ -991,15 +991,15 @@
 #[pyo3(text_signature = "(coeffs_left, coeffs_right, vars)")]
 fn mul_different_vars<'py>(
     py: Python<'py>,
     coeffs_left: PyReadonlyArrayDyn<f64>,
     coeffs_right: PyReadonlyArrayDyn<f64>,
     nvars_left: usize,
     nvars_right: usize,
-) -> PyResult<&'py PyArrayDyn<f64>> {
+) -> PyResult<Bound<'py, PyArrayDyn<f64>>> {
     let Some(ncoeffs_left) = coeffs_left.shape().last() else {
         return Err(PyValueError::new_err("expected `coeffs_left` with at least one axis"));
     };
     let Some(ncoeffs_right) = coeffs_right.shape().last() else {
         return Err(PyValueError::new_err("expected `coeffs_right` with at least one axis"));
     };
     let degree_left = degree(nvars_left, *ncoeffs_left)?;
@@ -1025,15 +1025,15 @@
 #[pyo3(text_signature = "(inner_coeffs, inner_nvars, outer_nvars, outer_degree)")]
 fn composition_with_inner_matrix<'py>(
     py: Python<'py>,
     inner_coeffs: PyReadonlyArray2<f64>,
     inner_nvars: usize,
     outer_nvars: usize,
     outer_degree: Power,
-) -> PyResult<&'py PyArray2<f64>> {
+) -> PyResult<Bound<'py, PyArray2<f64>>> {
     let inner_coeffs = inner_coeffs.as_array();
     if inner_coeffs.shape()[0] != outer_nvars {
         return Err(PyValueError::new_err(format!(
             "expected `inner_coeffs` with shape ({}, ?) but got ({}, {})",
             outer_nvars,
             inner_coeffs.shape()[0],
             inner_coeffs.shape()[1],
@@ -1049,15 +1049,15 @@
             .copied(),
         inner_nvars,
         inner_degree,
         outer_nvars,
         outer_degree,
     )
     .map_err(|err| PyValueError::new_err(err.to_string()))?;
-    Ok(result.to_pyarray(py))
+    Ok(result.to_pyarray_bound(py))
 }
 
 /// Return coefficients for the given degree.
 ///
 /// Given coefficients for a polynomial in ``nvars`` variables of implied
 /// degree ``old_degree``, this function returns coefficients for degree
 /// ``new_degree``.
@@ -1094,15 +1094,15 @@
 #[pyfunction]
 #[pyo3(text_signature = "(coeffs, nvars, new_degree)")]
 fn change_degree<'py>(
     py: Python<'py>,
     coeffs: PyReadonlyArrayDyn<f64>,
     nvars: usize,
     new_degree: Power,
-) -> PyResult<&'py PyArrayDyn<f64>> {
+) -> PyResult<Bound<'py, PyArrayDyn<f64>>> {
     let (coeffs, degree, _, leading_shape) = as_coeffs_dyn(&coeffs, nvars, "coeffs")?;
     let Some(new_indices) = nutils_poly::MapDegree::new(nvars, degree, new_degree) else {
         return Err(PyValueError::new_err(
             "the new degree is lower than the old degree",
         ));
     };
     // `MapDegree` is expensive. Since we are using `new_indices` multiple
@@ -1112,15 +1112,15 @@
     let new_shape = shape![leading_shape, [new_ncoeffs]];
     let mut new_coeffs: ArrayD<f64> = ArrayD::zeros(&new_shape[..]);
     for (mut new_coeffs, coeffs) in iter::zip(new_coeffs.rows_mut(), coeffs.rows()) {
         for (coeff, new_index) in iter::zip(coeffs, &new_indices) {
             new_coeffs[*new_index] = *coeff;
         }
     }
-    Ok(PyArray::from_owned_array(py, new_coeffs))
+    Ok(PyArray::from_owned_array_bound(py, new_coeffs))
 }
 
 /// Low-level functions for evaluating and manipulating polynomials.
 ///
 /// The polynomials considered in this module are `power series`_ in zero or
 /// more variables centered at zero and truncated to order :math:`p`,
 ///
@@ -1169,15 +1169,15 @@
 /// ...     [[2, 0, 3], [2, 2, 0]],
 /// ... )
 ///
 /// .. _power series: https://en.wikipedia.org/wiki/Power_series
 /// .. _lexicographic order: https://en.wikipedia.org/wiki/Lexicographic_order
 #[pymodule]
 #[pyo3(name = "nutils_poly")]
-fn pymod(_py: Python, m: &PyModule) -> PyResult<()> {
+fn pymod(_py: Python, m: &Bound<PyModule>) -> PyResult<()> {
     m.add_class::<PyMulVar>()?;
     m.add_class::<PyMulPlan>()?;
     m.add_class::<PyPartialDerivPlan>()?;
     m.add_class::<PyGradPlan>()?;
 
     macro_rules! wrap_and_add_pyfunctions {
         ($m:ident $(, $f:ident)* $(,)?) => {
```

### Comparing `nutils_poly-1.0.0/test.py` & `nutils_poly-1.0.1/test.py`

 * *Files identical despite different names*

### Comparing `nutils_poly-1.0.0/Cargo.lock` & `nutils_poly-1.0.1/Cargo.lock`

 * *Files 13% similar despite different names*

```diff
@@ -1,54 +1,43 @@
 # This file is automatically @generated by Cargo.
 # It is not intended for manual editing.
 version = 3
 
 [[package]]
-name = "ahash"
-version = "0.7.6"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fcb51a0695d8f838b1ee009b3fbf66bda078cd64590202a864a8f3e8c4315c47"
-dependencies = [
- "getrandom",
- "once_cell",
- "version_check",
-]
-
-[[package]]
 name = "autocfg"
-version = "1.1.0"
+version = "1.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d468802bab17cbc0cc575e9b053f41e72aa36bfa6b7f55e3529ffa43161b97fa"
+checksum = "0c4b4d0bd25bd0b74681c0ad21497610ce1b7c91b1022cd21c80c6fbdd9476b0"
 
 [[package]]
 name = "bitflags"
-version = "1.3.2"
+version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
+checksum = "cf4b9d6a944f767f8e5e0db018570623c85f3d925ac718db4e06d0187adb21c1"
 
 [[package]]
 name = "block-buffer"
-version = "0.10.3"
+version = "0.10.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "69cce20737498f97b993470a6e536b8523f0af7892a4f928cceb1ac5e52ebe7e"
+checksum = "3078c7629b62d3f0439517fa394996acacc5cbc91c5a20d8c658e77abd503a71"
 dependencies = [
  "generic-array",
 ]
 
 [[package]]
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
 name = "cpufeatures"
-version = "0.2.5"
+version = "0.2.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "28d997bd5e24a5928dd43e46dc529867e207907fe0b239c3477d924f7f2ca320"
+checksum = "53fe5e26ff1b7aef8bca9c6080520cfb8d9333c7568e1829cef191a9723e5504"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "crypto-common"
 version = "0.1.6"
@@ -57,79 +46,75 @@
 dependencies = [
  "generic-array",
  "typenum",
 ]
 
 [[package]]
 name = "digest"
-version = "0.10.6"
+version = "0.10.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8168378f4e5023e7218c89c891c0fd8ecdb5e5e4f18cb78f38cf245dd021e76f"
+checksum = "9ed9a281f7bc9b7576e61468ba615a66a5c8cfdff42420a70aa82701a3b1e292"
 dependencies = [
  "block-buffer",
  "crypto-common",
 ]
 
 [[package]]
 name = "generic-array"
-version = "0.14.6"
+version = "0.14.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bff49e947297f3312447abdca79f45f4738097cc82b06e72054d2223f601f1b9"
+checksum = "85649ca51fd72272d7821adaf274ad91c288277713d9c18820d8499a7ff69e9a"
 dependencies = [
  "typenum",
  "version_check",
 ]
 
 [[package]]
-name = "getrandom"
-version = "0.2.8"
+name = "heck"
+version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c05aeb6a22b8f62540c194aac980f2115af067bfe15a0734d7277a768d396b31"
-dependencies = [
- "cfg-if",
- "libc",
- "wasi",
-]
+checksum = "95505c38b4572b2d910cecb0281560f54b440a19336cbbcb27bf6ce6adc6f5a8"
 
 [[package]]
 name = "indoc"
-version = "1.0.8"
+version = "2.0.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "da2d6f23ffea9d7e76c53eee25dfb67bcd8fde7f1198b0855350698c9f07c780"
+checksum = "b248f5224d1d606005e02c97f5aa4e88eeb230488bcc03bc9ca4d7991399f2b5"
 
 [[package]]
 name = "libc"
-version = "0.2.139"
+version = "0.2.154"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "201de327520df007757c1f0adce6e827fe8562fbc28bfd9c15571c66ca1f5f79"
+checksum = "ae743338b92ff9146ce83992f766a31066a91a8c84a45e0e9f21e7cf6de6d346"
 
 [[package]]
 name = "lock_api"
-version = "0.4.9"
+version = "0.4.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "435011366fe56583b16cf956f9df0095b405b82d76425bc8981c0e22e60ec4df"
+checksum = "07af8b9cdd281b7915f413fa73f29ebd5d55d0d3f0155584dade1ff18cea1b17"
 dependencies = [
  "autocfg",
  "scopeguard",
 ]
 
 [[package]]
 name = "matrixmultiply"
-version = "0.3.2"
+version = "0.3.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "add85d4dd35074e6fedc608f8c8f513a3548619a9024b751949ef0e8e45a4d84"
+checksum = "7574c1cf36da4798ab73da5b215bbf444f50718207754cb522201d78d1cd0ff2"
 dependencies = [
+ "autocfg",
  "rawpointer",
 ]
 
 [[package]]
 name = "memoffset"
-version = "0.6.5"
+version = "0.9.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5aa361d4faea93603064a027415f07bd8e1d5c88c9fbf68bf56a285428fd79ce"
+checksum = "488016bfae457b036d996092f6cb448677611ce4449e970ceaf42695203f218a"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "ndarray"
 version = "0.15.6"
@@ -141,53 +126,52 @@
  "num-integer",
  "num-traits",
  "rawpointer",
 ]
 
 [[package]]
 name = "num-complex"
-version = "0.4.2"
+version = "0.4.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7ae39348c8bc5fbd7f40c727a9925f03517afd2ab27d46702108b6a7e5414c19"
+checksum = "23c6602fda94a57c990fe0df199a035d83576b496aa29f4e634a8ac6004e68a6"
 dependencies = [
  "num-traits",
 ]
 
 [[package]]
 name = "num-integer"
-version = "0.1.45"
+version = "0.1.46"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "225d3389fb3509a24c93f5c29eb6bde2586b98d9f016636dff58d7c6f7569cd9"
+checksum = "7969661fd2958a5cb096e56c8e1ad0444ac2bbcd0061bd28660485a44879858f"
 dependencies = [
- "autocfg",
  "num-traits",
 ]
 
 [[package]]
 name = "num-traits"
-version = "0.2.15"
+version = "0.2.19"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "578ede34cf02f8924ab9447f50c28075b4d3e5b269972345e7e0372b38c6cdcd"
+checksum = "071dfc062690e90b734c0b2273ce72ad0ffa95f0c74596bc250dcfd960262841"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "numpy"
-version = "0.17.2"
+version = "0.21.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a462c1af5ba1fddec1488c4646993a23ae7931f9e170ccba23e9c7c834277797"
+checksum = "ec170733ca37175f5d75a5bea5911d6ff45d2cd52849ce98b685394e4f2f37f4"
 dependencies = [
- "ahash",
  "libc",
  "ndarray",
  "num-complex",
  "num-integer",
  "num-traits",
  "pyo3",
+ "rustc-hash",
 ]
 
 [[package]]
 name = "nutils-poly"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1b9a8c1fa398bc3a94340c3bb3e722ff57f5a37034a4f30c1b2f34a8b18cd4d6"
@@ -195,274 +179,290 @@
  "ndarray",
  "num-traits",
  "sqnc",
 ]
 
 [[package]]
 name = "nutils-poly-py"
-version = "1.0.0"
+version = "1.0.1"
 dependencies = [
  "ndarray",
  "numpy",
  "nutils-poly",
  "pyo3",
  "sha1",
  "sqnc",
 ]
 
 [[package]]
 name = "once_cell"
-version = "1.17.0"
+version = "1.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6f61fba1741ea2b3d6a1e3178721804bb716a68a6aeba1149b5d52e3d464ea66"
+checksum = "3fdb12b2476b595f9358c5161aa467c2438859caa136dec86c26fdd2efe17b92"
 
 [[package]]
 name = "parking_lot"
-version = "0.12.1"
+version = "0.12.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3742b2c103b9f06bc9fff0a37ff4912935851bee6d36f3c02bcc755bcfec228f"
+checksum = "7e4af0ca4f6caed20e900d564c242b8e5d4903fdacf31d3daf527b66fe6f42fb"
 dependencies = [
  "lock_api",
  "parking_lot_core",
 ]
 
 [[package]]
 name = "parking_lot_core"
-version = "0.9.6"
+version = "0.9.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ba1ef8814b5c993410bb3adfad7a5ed269563e4a2f90c41f5d85be7fb47133bf"
+checksum = "1e401f977ab385c9e4e3ab30627d6f26d00e2c73eef317493c4ec6d468726cf8"
 dependencies = [
  "cfg-if",
  "libc",
  "redox_syscall",
  "smallvec",
- "windows-sys",
+ "windows-targets",
 ]
 
 [[package]]
+name = "portable-atomic"
+version = "1.6.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7170ef9988bc169ba16dd36a7fa041e5c4cbeb6a35b76d4c03daded371eae7c0"
+
+[[package]]
 name = "proc-macro2"
-version = "1.0.50"
+version = "1.0.82"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6ef7d57beacfaf2d8aee5937dab7b7f28de3cb8b1828479bb5de2a7106f2bae2"
+checksum = "8ad3d49ab951a01fbaafe34f2ec74122942fe18a3f9814c3268f1bb72042131b"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3"
-version = "0.17.3"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "268be0c73583c183f2b14052337465768c07726936a260f480f0857cb95ba543"
+checksum = "a5e00b96a521718e08e03b1a622f01c8a8deb50719335de3f60b3b3950f069d8"
 dependencies = [
  "cfg-if",
  "indoc",
  "libc",
  "memoffset",
  "parking_lot",
+ "portable-atomic",
  "pyo3-build-config",
  "pyo3-ffi",
  "pyo3-macros",
  "unindent",
 ]
 
 [[package]]
 name = "pyo3-build-config"
-version = "0.17.3"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "28fcd1e73f06ec85bf3280c48c67e731d8290ad3d730f8be9dc07946923005c8"
+checksum = "7883df5835fafdad87c0d888b266c8ec0f4c9ca48a5bed6bbb592e8dedee1b50"
 dependencies = [
  "once_cell",
  "target-lexicon",
 ]
 
 [[package]]
 name = "pyo3-ffi"
-version = "0.17.3"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0f6cb136e222e49115b3c51c32792886defbfb0adead26a688142b346a0b9ffc"
+checksum = "01be5843dc60b916ab4dad1dca6d20b9b4e6ddc8e15f50c47fe6d85f1fb97403"
 dependencies = [
  "libc",
  "pyo3-build-config",
 ]
 
 [[package]]
 name = "pyo3-macros"
-version = "0.17.3"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "94144a1266e236b1c932682136dc35a9dee8d3589728f68130c7c3861ef96b28"
+checksum = "77b34069fc0682e11b31dbd10321cbf94808394c56fd996796ce45217dfac53c"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
-version = "0.17.3"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c8df9be978a2d2f0cdebabb03206ed73b11314701a5bfe71b0d753b81997777f"
+checksum = "08260721f32db5e1a5beae69a55553f56b99bd0e1c3e6e0a5e8851a9d0f5a85c"
 dependencies = [
+ "heck",
  "proc-macro2",
+ "pyo3-build-config",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "quote"
-version = "1.0.23"
+version = "1.0.36"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8856d8364d252a14d474036ea1358d63c9e6965c8e5c1885c18f73d70bff9c7b"
+checksum = "0fa76aaf39101c457836aec0ce2316dbdc3ab723cdda1c6bd4e6ad4208acaca7"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "rawpointer"
 version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "60a357793950651c4ed0f3f52338f53b2f809f32d83a07f72909fa13e4c6c1e3"
 
 [[package]]
 name = "redox_syscall"
-version = "0.2.16"
+version = "0.5.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fb5a58c1855b4b6819d59012155603f0b22ad30cad752600aadfcb695265519a"
+checksum = "469052894dcb553421e483e4209ee581a45100d31b4018de03e5a7ad86374a7e"
 dependencies = [
  "bitflags",
 ]
 
 [[package]]
-name = "scopeguard"
+name = "rustc-hash"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d29ab0c6d3fc0ee92fe66e2d99f700eab17a8d57d1c1d3b748380fb20baa78cd"
+checksum = "08d43f7aa6b08d49f382cde6a7982047c3426db949b1424bc4b7ec9ae12c6ce2"
+
+[[package]]
+name = "scopeguard"
+version = "1.2.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "94143f37725109f92c262ed2cf5e59bce7498c01bcc1502d7b9afe439a4e9f49"
 
 [[package]]
 name = "sha1"
-version = "0.10.5"
+version = "0.10.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f04293dc80c3993519f2d7f6f511707ee7094fe0c6d3406feb330cdb3540eba3"
+checksum = "e3bf829a2d51ab4a5ddf1352d8470c140cadc8301b2ae1789db023f01cedd6ba"
 dependencies = [
  "cfg-if",
  "cpufeatures",
  "digest",
 ]
 
 [[package]]
 name = "smallvec"
-version = "1.10.0"
+version = "1.13.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a507befe795404456341dfab10cef66ead4c041f62b8b11bbb92bffe5d0953e0"
+checksum = "3c5e1a9a646d36c3599cd173a41282daf47c44583ad367b8e6837255952e5c67"
 
 [[package]]
 name = "sqnc"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7ea4c9c29903834c064ff1653bf2d52de869f2b1de109fdb1751308e53b192c1"
 dependencies = [
  "ndarray",
 ]
 
 [[package]]
 name = "syn"
-version = "1.0.107"
+version = "2.0.61"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1f4064b5b16e03ae50984a5a8ed5d4f8803e6bc1fd170a3cda91a1be4b18e3f5"
+checksum = "c993ed8ccba56ae856363b1845da7266a7cb78e1d146c8a32d54b45a8b831fc9"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "target-lexicon"
-version = "0.12.5"
+version = "0.12.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9410d0f6853b1d94f0e519fb95df60f29d2c1eff2d921ffdf01a4c8a3b54f12d"
+checksum = "e1fc403891a21bcfb7c37834ba66a547a8f402146eba7265b5a6d88059c9ff2f"
 
 [[package]]
 name = "typenum"
-version = "1.16.0"
+version = "1.17.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "497961ef93d974e23eb6f433eb5fe1b7930b659f06d12dec6fc44a8f554c0bba"
+checksum = "42ff0bf0c66b8238c6f3b578df37d0b7848e55df8577b3f74f92a69acceeb825"
 
 [[package]]
 name = "unicode-ident"
-version = "1.0.6"
+version = "1.0.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "84a22b9f218b40614adcb3f4ff08b703773ad44fa9423e4e0d346d5db86e4ebc"
+checksum = "3354b9ac3fae1ff6755cb6db53683adb661634f67557942dea4facebec0fee4b"
 
 [[package]]
 name = "unindent"
-version = "0.1.11"
+version = "0.2.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e1766d682d402817b5ac4490b3c3002d91dfa0d22812f341609f97b08757359c"
+checksum = "c7de7d73e1754487cb58364ee906a499937a0dfabd86bcb980fa99ec8c8fa2ce"
 
 [[package]]
 name = "version_check"
 version = "0.9.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "49874b5167b65d7193b8aba1567f5c7d93d001cafc34600cee003eda787e483f"
 
 [[package]]
-name = "wasi"
-version = "0.11.0+wasi-snapshot-preview1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9c8d87e72b64a3b4db28d11ce29237c246188f4f51057d65a7eab63b7987e423"
-
-[[package]]
-name = "windows-sys"
-version = "0.42.0"
+name = "windows-targets"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5a3e1820f08b8513f676f7ab6c1f99ff312fb97b553d30ff4dd86f9f15728aa7"
+checksum = "6f0713a46559409d202e70e28227288446bf7841d3211583a4b53e3f6d96e7eb"
 dependencies = [
  "windows_aarch64_gnullvm",
  "windows_aarch64_msvc",
  "windows_i686_gnu",
+ "windows_i686_gnullvm",
  "windows_i686_msvc",
  "windows_x86_64_gnu",
  "windows_x86_64_gnullvm",
  "windows_x86_64_msvc",
 ]
 
 [[package]]
 name = "windows_aarch64_gnullvm"
-version = "0.42.1"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8c9864e83243fdec7fc9c5444389dcbbfd258f745e7853198f365e3c4968a608"
+checksum = "7088eed71e8b8dda258ecc8bac5fb1153c5cffaf2578fc8ff5d61e23578d3263"
 
 [[package]]
 name = "windows_aarch64_msvc"
-version = "0.42.1"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4c8b1b673ffc16c47a9ff48570a9d85e25d265735c503681332589af6253c6c7"
+checksum = "9985fd1504e250c615ca5f281c3f7a6da76213ebd5ccc9561496568a2752afb6"
 
 [[package]]
 name = "windows_i686_gnu"
-version = "0.42.1"
+version = "0.52.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "88ba073cf16d5372720ec942a8ccbf61626074c6d4dd2e745299726ce8b89670"
+
+[[package]]
+name = "windows_i686_gnullvm"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "de3887528ad530ba7bdbb1faa8275ec7a1155a45ffa57c37993960277145d640"
+checksum = "87f4261229030a858f36b459e748ae97545d6f1ec60e5e0d6a3d32e0dc232ee9"
 
 [[package]]
 name = "windows_i686_msvc"
-version = "0.42.1"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bf4d1122317eddd6ff351aa852118a2418ad4214e6613a50e0191f7004372605"
+checksum = "db3c2bf3d13d5b658be73463284eaf12830ac9a26a90c717b7f771dfe97487bf"
 
 [[package]]
 name = "windows_x86_64_gnu"
-version = "0.42.1"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c1040f221285e17ebccbc2591ffdc2d44ee1f9186324dd3e84e99ac68d699c45"
+checksum = "4e4246f76bdeff09eb48875a0fd3e2af6aada79d409d33011886d3e1581517d9"
 
 [[package]]
 name = "windows_x86_64_gnullvm"
-version = "0.42.1"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "628bfdf232daa22b0d64fdb62b09fcc36bb01f05a3939e20ab73aaf9470d0463"
+checksum = "852298e482cd67c356ddd9570386e2862b5673c85bd5f88df9ab6802b334c596"
 
 [[package]]
 name = "windows_x86_64_msvc"
-version = "0.42.1"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "447660ad36a13288b1db4d4248e857b510e8c3a225c822ba4fb748c0aafecffd"
+checksum = "bec47e5bfd1bff0eeaf6d8b485cc1074891a197ab4225d504cb7a1ab88b02bf0"
```

### Comparing `nutils_poly-1.0.0/PKG-INFO` & `nutils_poly-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: nutils-poly
-Version: 1.0.0
+Version: 1.0.1
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Dist: numpy
 Summary: Low-level functions for evaluating and manipulating polynomials (Python bindings)
 Author: Evalf <info@evalf.com>
 Author-email: Evalf <info@evalf.com>
 License: MIT
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 Project-URL: repository, https://github.com/nutils/poly-py
 
 Low-level functions for evaluating and manipulating polynomials.
 
 # Examples
```

