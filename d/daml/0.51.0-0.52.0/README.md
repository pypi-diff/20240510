# Comparing `tmp/daml-0.51.0.tar.gz` & `tmp/daml-0.52.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "daml-0.51.0.tar", max compression
+gzip compressed data, was "daml-0.52.0.tar", max compression
```

## Comparing `daml-0.51.0.tar` & `daml-0.52.0.tar`

### file list

```diff
@@ -1,61 +1,49 @@
--rw-r--r--   0        0        0     1060 2024-04-26 03:05:58.911849 daml-0.51.0/LICENSE.txt
--rw-r--r--   0        0        0     2528 2024-04-26 03:05:58.911849 daml-0.51.0/README.md
--rw-r--r--   0        0        0     5218 2024-04-26 03:06:03.903852 daml-0.51.0/pyproject.toml
--rw-r--r--   0        0        0      230 2024-04-26 03:06:03.907852 daml-0.51.0/src/daml/__init__.py
--rw-r--r--   0        0        0      115 2024-04-26 03:05:58.915849 daml-0.51.0/src/daml/_alibi_detect/__init__.py
--rw-r--r--   0        0        0     8269 2024-04-26 03:05:58.919849 daml-0.51.0/src/daml/_alibi_detect/base.py
--rw-r--r--   0        0        0        0 2024-04-26 03:05:58.919849 daml-0.51.0/src/daml/_alibi_detect/models/__init__.py
--rw-r--r--   0        0        0        0 2024-04-26 03:05:58.919849 daml-0.51.0/src/daml/_alibi_detect/models/tensorflow/__init__.py
--rw-r--r--   0        0        0    14452 2024-04-26 03:05:58.919849 daml-0.51.0/src/daml/_alibi_detect/models/tensorflow/autoencoder.py
--rw-r--r--   0        0        0     3207 2024-04-26 03:05:58.919849 daml-0.51.0/src/daml/_alibi_detect/models/tensorflow/gmm.py
--rw-r--r--   0        0        0     7823 2024-04-26 03:05:58.919849 daml-0.51.0/src/daml/_alibi_detect/models/tensorflow/losses.py
--rw-r--r--   0        0        0    49533 2024-04-26 03:05:58.919849 daml-0.51.0/src/daml/_alibi_detect/models/tensorflow/pixelcnn.py
--rw-r--r--   0        0        0     4332 2024-04-26 03:05:58.919849 daml-0.51.0/src/daml/_alibi_detect/models/tensorflow/trainer.py
--rw-r--r--   0        0        0      348 2024-04-26 03:05:58.919849 daml-0.51.0/src/daml/_alibi_detect/od/__init__.py
--rw-r--r--   0        0        0     9375 2024-04-26 03:05:58.919849 daml-0.51.0/src/daml/_alibi_detect/od/ae.py
--rw-r--r--   0        0        0     7797 2024-04-26 03:05:58.919849 daml-0.51.0/src/daml/_alibi_detect/od/aegmm.py
--rw-r--r--   0        0        0    14179 2024-04-26 03:05:58.919849 daml-0.51.0/src/daml/_alibi_detect/od/llr.py
--rw-r--r--   0        0        0    11453 2024-04-26 03:05:58.919849 daml-0.51.0/src/daml/_alibi_detect/od/vae.py
--rw-r--r--   0        0        0     9801 2024-04-26 03:05:58.919849 daml-0.51.0/src/daml/_alibi_detect/od/vaegmm.py
--rw-r--r--   0        0        0        0 2024-04-26 03:05:58.919849 daml-0.51.0/src/daml/_alibi_detect/utils/__init__.py
--rw-r--r--   0        0        0     1758 2024-04-26 03:05:58.919849 daml-0.51.0/src/daml/_alibi_detect/utils/_types.py
--rw-r--r--   0        0        0     5269 2024-04-26 03:05:58.919849 daml-0.51.0/src/daml/_alibi_detect/utils/frameworks.py
--rw-r--r--   0        0        0     5410 2024-04-26 03:05:58.919849 daml-0.51.0/src/daml/_alibi_detect/utils/missing_optional_dependency.py
--rw-r--r--   0        0        0      647 2024-04-26 03:05:58.919849 daml-0.51.0/src/daml/_alibi_detect/utils/prediction.py
--rw-r--r--   0        0        0        0 2024-04-26 03:05:58.919849 daml-0.51.0/src/daml/_alibi_detect/utils/tensorflow/__init__.py
--rw-r--r--   0        0        0     9525 2024-04-26 03:05:58.919849 daml-0.51.0/src/daml/_alibi_detect/utils/tensorflow/distance.py
--rw-r--r--   0        0        0     1096 2024-04-26 03:05:58.919849 daml-0.51.0/src/daml/_alibi_detect/utils/tensorflow/perturbation.py
--rw-r--r--   0        0        0     3522 2024-04-26 03:05:58.919849 daml-0.51.0/src/daml/_alibi_detect/utils/tensorflow/prediction.py
--rw-r--r--   0        0        0      217 2024-04-26 03:05:58.919849 daml-0.51.0/src/daml/_alibi_detect/version.py
--rw-r--r--   0        0        0        0 2024-04-26 03:05:58.919849 daml-0.51.0/src/daml/_internal/metrics/__init__.py
--rw-r--r--   0        0        0     2442 2024-04-26 03:05:58.919849 daml-0.51.0/src/daml/_internal/metrics/base.py
--rw-r--r--   0        0        0     2912 2024-04-26 03:05:58.919849 daml-0.51.0/src/daml/_internal/metrics/ber.py
--rw-r--r--   0        0        0     2819 2024-04-26 03:05:58.919849 daml-0.51.0/src/daml/_internal/metrics/divergence.py
--rw-r--r--   0        0        0        0 2024-04-26 03:05:58.919849 daml-0.51.0/src/daml/_internal/metrics/drift/__init__.py
--rw-r--r--   0        0        0     8981 2024-04-26 03:05:58.919849 daml-0.51.0/src/daml/_internal/metrics/drift/base.py
--rw-r--r--   0        0        0     3897 2024-04-26 03:05:58.919849 daml-0.51.0/src/daml/_internal/metrics/drift/cvm.py
--rw-r--r--   0        0        0     3954 2024-04-26 03:05:58.919849 daml-0.51.0/src/daml/_internal/metrics/drift/ks.py
--rw-r--r--   0        0        0     7199 2024-04-26 03:05:58.919849 daml-0.51.0/src/daml/_internal/metrics/drift/mmd.py
--rw-r--r--   0        0        0    10972 2024-04-26 03:05:58.919849 daml-0.51.0/src/daml/_internal/metrics/drift/torch.py
--rw-r--r--   0        0        0     5285 2024-04-26 03:05:58.919849 daml-0.51.0/src/daml/_internal/metrics/drift/uncertainty.py
--rw-r--r--   0        0        0    15892 2024-04-26 03:05:58.919849 daml-0.51.0/src/daml/_internal/metrics/od.py
--rw-r--r--   0        0        0    13841 2024-04-26 03:05:58.919849 daml-0.51.0/src/daml/_internal/metrics/sufficiency.py
--rw-r--r--   0        0        0     1167 2024-04-26 03:05:58.919849 daml-0.51.0/src/daml/_internal/metrics/uap.py
--rw-r--r--   0        0        0     2316 2024-04-26 03:05:58.919849 daml-0.51.0/src/daml/_internal/metrics/utils.py
--rw-r--r--   0        0        0        0 2024-04-26 03:05:58.919849 daml-0.51.0/src/daml/_internal/models/__init__.py
--rw-r--r--   0        0        0        0 2024-04-26 03:05:58.919849 daml-0.51.0/src/daml/_internal/models/pytorch/__init__.py
--rw-r--r--   0        0        0     6240 2024-04-26 03:05:58.919849 daml-0.51.0/src/daml/_internal/models/pytorch/autoencoder.py
--rw-r--r--   0        0        0     1354 2024-04-26 03:05:58.919849 daml-0.51.0/src/daml/_internal/models/pytorch/blocks.py
--rw-r--r--   0        0        0     1675 2024-04-26 03:05:58.919849 daml-0.51.0/src/daml/_internal/models/pytorch/utils.py
--rw-r--r--   0        0        0        0 2024-04-26 03:05:58.919849 daml-0.51.0/src/daml/_internal/models/tensorflow/__init__.py
--rw-r--r--   0        0        0     5107 2024-04-26 03:05:58.919849 daml-0.51.0/src/daml/_internal/models/tensorflow/alibi.py
--rw-r--r--   0        0        0      856 2024-04-26 03:05:58.919849 daml-0.51.0/src/daml/_prototype/README.md
--rw-r--r--   0        0        0     7453 2024-04-26 03:05:58.919849 daml-0.51.0/src/daml/_prototype/cleaning.py
--rw-r--r--   0        0        0     4544 2024-04-26 03:05:58.919849 daml-0.51.0/src/daml/_prototype/linting.py
--rw-r--r--   0        0        0      626 2024-04-26 03:05:58.919849 daml-0.51.0/src/daml/metrics/__init__.py
--rw-r--r--   0        0        0      678 2024-04-26 03:05:58.919849 daml-0.51.0/src/daml/metrics/drift/__init__.py
--rw-r--r--   0        0        0      303 2024-04-26 03:05:58.919849 daml-0.51.0/src/daml/metrics/outlier_detection/__init__.py
--rw-r--r--   0        0        0      151 2024-04-26 03:05:58.919849 daml-0.51.0/src/daml/models/__init__.py
--rw-r--r--   0        0        0      186 2024-04-26 03:05:58.919849 daml-0.51.0/src/daml/models/ae/__init__.py
--rw-r--r--   0        0        0        0 2024-04-26 03:05:58.919849 daml-0.51.0/src/daml/py.typed
--rw-r--r--   0        0        0     5034 1970-01-01 00:00:00.000000 daml-0.51.0/PKG-INFO
+-rw-r--r--   0        0        0     1060 2024-05-10 03:05:41.196777 daml-0.52.0/LICENSE.txt
+-rw-r--r--   0        0        0     2528 2024-05-10 03:05:41.196777 daml-0.52.0/README.md
+-rw-r--r--   0        0        0     5170 2024-05-10 03:05:55.524837 daml-0.52.0/pyproject.toml
+-rw-r--r--   0        0        0      230 2024-05-10 03:05:55.528838 daml-0.52.0/src/daml/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-10 03:05:41.204777 daml-0.52.0/src/daml/_internal/metrics/__init__.py
+-rw-r--r--   0        0        0     2412 2024-05-10 03:05:41.204777 daml-0.52.0/src/daml/_internal/metrics/base.py
+-rw-r--r--   0        0        0     2912 2024-05-10 03:05:41.204777 daml-0.52.0/src/daml/_internal/metrics/ber.py
+-rw-r--r--   0        0        0     2819 2024-05-10 03:05:41.204777 daml-0.52.0/src/daml/_internal/metrics/divergence.py
+-rw-r--r--   0        0        0        0 2024-05-10 03:05:41.204777 daml-0.52.0/src/daml/_internal/metrics/drift/__init__.py
+-rw-r--r--   0        0        0     8981 2024-05-10 03:05:41.204777 daml-0.52.0/src/daml/_internal/metrics/drift/base.py
+-rw-r--r--   0        0        0     3897 2024-05-10 03:05:41.204777 daml-0.52.0/src/daml/_internal/metrics/drift/cvm.py
+-rw-r--r--   0        0        0     3924 2024-05-10 03:05:41.204777 daml-0.52.0/src/daml/_internal/metrics/drift/ks.py
+-rw-r--r--   0        0        0     6965 2024-05-10 03:05:41.204777 daml-0.52.0/src/daml/_internal/metrics/drift/mmd.py
+-rw-r--r--   0        0        0    10866 2024-05-10 03:05:41.204777 daml-0.52.0/src/daml/_internal/metrics/drift/torch.py
+-rw-r--r--   0        0        0     5263 2024-05-10 03:05:41.204777 daml-0.52.0/src/daml/_internal/metrics/drift/uncertainty.py
+-rw-r--r--   0        0        0        0 2024-05-10 03:05:41.204777 daml-0.52.0/src/daml/_internal/metrics/outlier/__init__.py
+-rw-r--r--   0        0        0     2596 2024-05-10 03:05:41.204777 daml-0.52.0/src/daml/_internal/metrics/outlier/ae.py
+-rw-r--r--   0        0        0     2364 2024-05-10 03:05:41.204777 daml-0.52.0/src/daml/_internal/metrics/outlier/aegmm.py
+-rw-r--r--   0        0        0     6831 2024-05-10 03:05:41.204777 daml-0.52.0/src/daml/_internal/metrics/outlier/base.py
+-rw-r--r--   0        0        0    10089 2024-05-10 03:05:41.204777 daml-0.52.0/src/daml/_internal/metrics/outlier/llr.py
+-rw-r--r--   0        0        0     2920 2024-05-10 03:05:41.204777 daml-0.52.0/src/daml/_internal/metrics/outlier/vae.py
+-rw-r--r--   0        0        0     2790 2024-05-10 03:05:41.204777 daml-0.52.0/src/daml/_internal/metrics/outlier/vaegmm.py
+-rw-r--r--   0        0        0    13549 2024-05-10 03:05:41.204777 daml-0.52.0/src/daml/_internal/metrics/sufficiency.py
+-rw-r--r--   0        0        0     1145 2024-05-10 03:05:41.204777 daml-0.52.0/src/daml/_internal/metrics/uap.py
+-rw-r--r--   0        0        0     2316 2024-05-10 03:05:41.204777 daml-0.52.0/src/daml/_internal/metrics/utils.py
+-rw-r--r--   0        0        0        0 2024-05-10 03:05:41.204777 daml-0.52.0/src/daml/_internal/models/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-10 03:05:41.204777 daml-0.52.0/src/daml/_internal/models/pytorch/__init__.py
+-rw-r--r--   0        0        0     6123 2024-05-10 03:05:41.204777 daml-0.52.0/src/daml/_internal/models/pytorch/autoencoder.py
+-rw-r--r--   0        0        0     1354 2024-05-10 03:05:41.204777 daml-0.52.0/src/daml/_internal/models/pytorch/blocks.py
+-rw-r--r--   0        0        0     1675 2024-05-10 03:05:41.204777 daml-0.52.0/src/daml/_internal/models/pytorch/utils.py
+-rw-r--r--   0        0        0        0 2024-05-10 03:05:41.204777 daml-0.52.0/src/daml/_internal/models/tensorflow/__init__.py
+-rw-r--r--   0        0        0    10008 2024-05-10 03:05:41.204777 daml-0.52.0/src/daml/_internal/models/tensorflow/autoencoder.py
+-rw-r--r--   0        0        0     3640 2024-05-10 03:05:41.204777 daml-0.52.0/src/daml/_internal/models/tensorflow/gmm.py
+-rw-r--r--   0        0        0     3776 2024-05-10 03:05:41.204777 daml-0.52.0/src/daml/_internal/models/tensorflow/losses.py
+-rw-r--r--   0        0        0    48091 2024-05-10 03:05:41.204777 daml-0.52.0/src/daml/_internal/models/tensorflow/pixelcnn.py
+-rw-r--r--   0        0        0     4113 2024-05-10 03:05:41.204777 daml-0.52.0/src/daml/_internal/models/tensorflow/trainer.py
+-rw-r--r--   0        0        0     8613 2024-05-10 03:05:41.204777 daml-0.52.0/src/daml/_internal/models/tensorflow/utils.py
+-rw-r--r--   0        0        0      856 2024-05-10 03:05:41.204777 daml-0.52.0/src/daml/_prototype/README.md
+-rw-r--r--   0        0        0     7273 2024-05-10 03:05:41.204777 daml-0.52.0/src/daml/_prototype/cleaning.py
+-rw-r--r--   0        0        0    21662 2024-05-10 03:05:41.204777 daml-0.52.0/src/daml/_prototype/linting.py
+-rw-r--r--   0        0        0    22416 2024-05-10 03:05:41.204777 daml-0.52.0/src/daml/_prototype/test_linting.ipynb
+-rw-r--r--   0        0        0      594 2024-05-10 03:05:41.204777 daml-0.52.0/src/daml/metrics/__init__.py
+-rw-r--r--   0        0        0      678 2024-05-10 03:05:41.204777 daml-0.52.0/src/daml/metrics/drift/__init__.py
+-rw-r--r--   0        0        0      488 2024-05-10 03:05:41.208778 daml-0.52.0/src/daml/metrics/outlier/__init__.py
+-rw-r--r--   0        0        0      293 2024-05-10 03:05:41.208778 daml-0.52.0/src/daml/models/__init__.py
+-rw-r--r--   0        0        0      408 2024-05-10 03:05:41.208778 daml-0.52.0/src/daml/models/tensorflow/__init__.py
+-rw-r--r--   0        0        0      186 2024-05-10 03:05:41.208778 daml-0.52.0/src/daml/models/torch/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-10 03:05:41.208778 daml-0.52.0/src/daml/py.typed
+-rw-r--r--   0        0        0     5034 1970-01-01 00:00:00.000000 daml-0.52.0/PKG-INFO
```

### Comparing `daml-0.51.0/LICENSE.txt` & `daml-0.52.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `daml-0.51.0/README.md` & `daml-0.52.0/README.md`

 * *Files identical despite different names*

### Comparing `daml-0.51.0/pyproject.toml` & `daml-0.52.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "daml"
-version = "0.51.0" # dynamic
+version = "0.52.0" # dynamic
 description = "DAML provides a simple interface to characterize image data and its impact on model performance across classification and object-detection tasks"
 license = "MIT"
 readme = "README.md"
 homepage = "https://daml.ai/"
 repository = "https://github.com/aria-ml/daml/"
 documentation = "https://daml.readthedocs.io/"
 
@@ -113,15 +113,14 @@
 pattern = "v(?P<base>\\d+\\.\\d+\\.\\d+)$"
 
 [tool.poetry-dynamic-versioning.substitution]
 files = ["src/daml/__init__.py"]
 
 [tool.pyright]
 reportMissingImports = false
-exclude = ["src/daml/_alibi_detect"]
 
 [tool.pytest.ini_options]
 markers = [
   "interop: marks external library interop tests",
   "functional: marks slower functional tests",
 ]
 
@@ -130,18 +129,17 @@
 exclude = [
   ".devcontainer",
   ".github",
   ".vscode",
   ".jupyter_cache",
   "*env*",
   "output",
-  "_alibi_detect",
   "_build"
 ]
-line-length = 88
+line-length = 120
 indent-width = 4
 target-version = "py38"
 extend-include = ["*.ipynb"]
 
 [tool.ruff.lint]
 select = ["A", "E", "F", "C4", "I", "UP", "NPY", "SIM", "RUF100"]
 ignore = ["NPY002"]
@@ -158,12 +156,12 @@
 indent-style = "space"
 skip-magic-trailing-comma = false
 line-ending = "auto"
 docstring-code-format = true
 docstring-code-line-length = "dynamic"
 
 [tool.codespell]
-skip = '*env*,docs/.jupyter_cache,CHANGELOG.md,poetry.lock,output'
+skip = '*env*,docs/.jupyter_cache,CHANGELOG.md,poetry.lock,output,*.html'
 
 [build-system]
 requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning"]
 build-backend = "poetry_dynamic_versioning.backend"
```

### Comparing `daml-0.51.0/src/daml/_alibi_detect/models/tensorflow/gmm.py` & `daml-0.52.0/src/daml/_internal/models/tensorflow/gmm.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,114 +1,115 @@
-from typing import Tuple
+"""
+Source code derived from Alibi-Detect 0.11.4
+https://github.com/SeldonIO/alibi-detect/tree/v0.11.4
+
+Original code Copyright (c) 2023 Seldon Technologies Ltd
+Licensed under Apache Software License (Apache 2.0)
+"""
+
+from typing import NamedTuple, Tuple
 
 import numpy as np
 import tensorflow as tf
 
 
-def gmm_params(
-    z: tf.Tensor, gamma: tf.Tensor
-) -> Tuple[tf.Tensor, tf.Tensor, tf.Tensor, tf.Tensor, tf.Tensor]:
+class GaussianMixtureModelParams(NamedTuple):
+    """
+    phi : tf.Tensor
+        Mixture component distribution weights.
+    mu : tf.Tensor
+        Mixture means.
+    cov : tf.Tensor
+        Mixture covariance.
+    L : tf.Tensor
+        Cholesky decomposition of `cov`.
+    log_det_cov : tf.Tensor
+        Log of the determinant of `cov`.
+    """
+
+    phi: tf.Tensor
+    mu: tf.Tensor
+    cov: tf.Tensor
+    L: tf.Tensor
+    log_det_cov: tf.Tensor
+
+
+def gmm_params(z: tf.Tensor, gamma: tf.Tensor) -> GaussianMixtureModelParams:
     """
     Compute parameters of Gaussian Mixture Model.
 
     Parameters
     ----------
-    z
+    z : tf.Tensor
         Observations.
-    gamma
+    gamma : tf.Tensor
         Mixture probabilities to derive mixture distribution weights from.
 
     Returns
     -------
-    phi
-        Mixture component distribution weights.
-    mu
-        Mixture means.
-    cov
-        Mixture covariance.
-    L
-        Cholesky decomposition of `cov`.
-    log_det_cov
-        Log of the determinant of `cov`.
+    GaussianMixtureModelParams(phi, mu, cov, L, log_det_cov)
+        The parameters used to calculate energy.
     """
     # compute gmm parameters phi, mu and cov
     N = gamma.shape[0]  # nb of samples in batch
     sum_gamma = tf.reduce_sum(gamma, 0)  # K
     phi = sum_gamma / N  # K
-    mu = tf.reduce_sum(
-        tf.expand_dims(gamma, -1) * tf.expand_dims(z, 1), 0
-    ) / tf.expand_dims(
+    mu = tf.reduce_sum(tf.expand_dims(gamma, -1) * tf.expand_dims(z, 1), 0) / tf.expand_dims(
         sum_gamma, -1
     )  # K x D (D = latent_dim)
     z_mu = tf.expand_dims(z, 1) - tf.expand_dims(mu, 0)  # N x K x D
     z_mu_outer = tf.expand_dims(z_mu, -1) * tf.expand_dims(z_mu, -2)  # N x K x D x D
-    cov = tf.reduce_sum(
-        tf.expand_dims(tf.expand_dims(gamma, -1), -1) * z_mu_outer, 0
-    ) / tf.expand_dims(
+    cov = tf.reduce_sum(tf.expand_dims(tf.expand_dims(gamma, -1), -1) * z_mu_outer, 0) / tf.expand_dims(
         tf.expand_dims(sum_gamma, -1), -1
     )  # K x D x D
 
     # cholesky decomposition of covariance and determinant derivation
-    D = tf.shape(cov)[1]
+    D = tf.shape(cov)[1]  # type: ignore
     eps = 1e-6
     L = tf.linalg.cholesky(cov + tf.eye(D) * eps)  # K x D x D
     log_det_cov = 2.0 * tf.reduce_sum(tf.math.log(tf.linalg.diag_part(L)), 1)  # K
 
-    return phi, mu, cov, L, log_det_cov
+    return GaussianMixtureModelParams(phi, mu, cov, L, log_det_cov)
 
 
 def gmm_energy(
     z: tf.Tensor,
-    phi: tf.Tensor,
-    mu: tf.Tensor,
-    cov: tf.Tensor,
-    L: tf.Tensor,
-    log_det_cov: tf.Tensor,
+    params: GaussianMixtureModelParams,
     return_mean: bool = True,
 ) -> Tuple[tf.Tensor, tf.Tensor]:
     """
     Compute sample energy from Gaussian Mixture Model.
 
     Parameters
     ----------
-    z
-        Observations.
-    phi
-        Mixture component distribution weights.
-    mu
-        Mixture means.
-    cov
-        Mixture covariance.
-    L
-        Cholesky decomposition of `cov`.
-    log_det_cov
-        Log of the determinant of `cov`.
-    return_mean
+    params : GaussianMixtureModelParams
+        The gaussian mixture model parameters.
+    return_mean : bool, default True
         Take mean across all sample energies in a batch.
 
     Returns
     -------
     sample_energy
         The sample energy of the GMM.
     cov_diag
         The inverse sum of the diagonal components of the covariance matrix.
     """
-    D = tf.shape(cov)[1]
-    z_mu = tf.expand_dims(z, 1) - tf.expand_dims(mu, 0)  # N x K x D
+    D = tf.shape(params.cov)[1]  # type: ignore
+    z_mu = tf.expand_dims(z, 1) - tf.expand_dims(params.mu, 0)  # N x K x D
     z_mu_T = tf.transpose(z_mu, perm=[1, 2, 0])  # K x D x N
-    v = tf.linalg.triangular_solve(L, z_mu_T, lower=True)  # K x D x D
+    v = tf.linalg.triangular_solve(params.L, z_mu_T, lower=True)  # K x D x D
 
     # rewrite sample energy in logsumexp format for numerical stability
-    logits = tf.math.log(tf.expand_dims(phi, -1)) - 0.5 * (
+    logits = tf.math.log(tf.expand_dims(params.phi, -1)) - 0.5 * (
         tf.reduce_sum(tf.square(v), 1)
-        + tf.cast(D, tf.float32) * tf.math.log(2.0 * np.pi)
-        + tf.expand_dims(log_det_cov, -1)
+        + tf.cast(D, tf.float32) * tf.math.log(2.0 * np.pi)  # type: ignore py38
+        + tf.expand_dims(params.log_det_cov, -1)
     )  # K x N
     sample_energy = -tf.reduce_logsumexp(logits, axis=0)  # N
 
     if return_mean:
         sample_energy = tf.reduce_mean(sample_energy)
 
     # inverse sum of variances
-    cov_diag = tf.reduce_sum(tf.divide(1, tf.linalg.diag_part(cov)))
+    cov_diag = tf.reduce_sum(tf.divide(1, tf.linalg.diag_part(params.cov)))
 
     return sample_energy, cov_diag
```

### Comparing `daml-0.51.0/src/daml/_alibi_detect/models/tensorflow/pixelcnn.py` & `daml-0.52.0/src/daml/_internal/models/tensorflow/pixelcnn.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,24 @@
-from __future__ import absolute_import, division, print_function
+# type: ignore
+
+"""
+Source code derived from Alibi-Detect 0.11.4
+https://github.com/SeldonIO/alibi-detect/tree/v0.11.4
+
+Original code Copyright (c) 2023 Seldon Technologies Ltd
+Licensed under Apache Software License (Apache 2.0)
+"""
 
 import functools
 import warnings
+from typing import Optional
 
+import keras.api._v2.keras as keras
 import numpy as np
-import tensorflow.compat.v2 as tf
+import tensorflow as tf
 from tensorflow_probability.python.bijectors import bijector
 from tensorflow_probability.python.distributions import (
     categorical,
     distribution,
     independent,
     logistic,
     mixture_same_family,
@@ -24,77 +34,70 @@
 )
 
 __all__ = [
     "Shift",
 ]
 
 
-class WeightNorm(tf.keras.layers.Wrapper):
+class WeightNorm(keras.layers.Wrapper):
     def __init__(self, layer, data_init: bool = True, **kwargs):
         """Layer wrapper to decouple magnitude and direction of the layer's weights.
 
         This wrapper reparameterizes a layer by decoupling the weight's
         magnitude and direction. This speeds up convergence by improving the
         conditioning of the optimization problem. It has an optional data-dependent
         initialization scheme, in which initial values of weights are set as functions
         of the first minibatch of data. Both the weight normalization and data-
         dependent initialization are described in [Salimans and Kingma (2016)][1].
 
         Parameters
         ----------
         layer
-            A `tf.keras.layers.Layer` instance. Supported layer types are
+            A `keras.layers.Layer` instance. Supported layer types are
             `Dense`, `Conv2D`, and `Conv2DTranspose`. Layers with multiple inputs
             are not supported.
         data_init
             If `True` use data dependent variable initialization.
         **kwargs
-            Additional keyword args passed to `tf.keras.layers.Wrapper`.
+            Additional keyword args passed to `keras.layers.Wrapper`.
 
         Raises
         ------
         ValueError
-            If `layer` is not a `tf.keras.layers.Layer` instance.
+            If `layer` is not a `keras.layers.Layer` instance.
         """
-        if not isinstance(layer, tf.keras.layers.Layer):
+        if not isinstance(layer, keras.layers.Layer):
             raise ValueError(
-                "Please initialize `WeightNorm` layer with a `tf.keras.layers.Layer` "
-                "instance. You passed: {input}".format(input=layer)
+                "Please initialize `WeightNorm` layer with a `keras.layers.Layer` " f"instance. You passed: {layer}"
             )
 
         layer_type = type(layer).__name__
         if layer_type not in ["Dense", "Conv2D", "Conv2DTranspose"]:
             warnings.warn(
                 "`WeightNorm` is tested only for `Dense`, `Conv2D`, and "
-                "`Conv2DTranspose` layers. You passed a layer of type `{}`".format(
-                    layer_type
-                )
+                f"`Conv2DTranspose` layers. You passed a layer of type `{layer_type}`"
             )
 
-        super(WeightNorm, self).__init__(layer, **kwargs)
+        super().__init__(layer, **kwargs)
 
         self.data_init = data_init
         self._track_trackable(layer, name="layer")
         self.filter_axis = -2 if layer_type == "Conv2DTranspose" else -1
 
     def _compute_weights(self):
         """Generate weights with normalization."""
         # Determine the axis along which to expand `g` so that `g` broadcasts to
         # the shape of `v`.
         new_axis = -self.filter_axis - 3
 
-        self.layer.kernel = tf.nn.l2_normalize(
-            self.v, axis=self.kernel_norm_axes
-        ) * tf.expand_dims(self.g, new_axis)
+        self.layer.kernel = tf.nn.l2_normalize(self.v, axis=self.kernel_norm_axes) * tf.expand_dims(self.g, new_axis)
 
     def _init_norm(self):
         """Set the norm of the weight vector."""
-        kernel_norm = tf.sqrt(
-            tf.reduce_sum(tf.square(self.v), axis=self.kernel_norm_axes)
-        )
+        kernel_norm = tf.sqrt(tf.reduce_sum(tf.square(self.v), axis=self.kernel_norm_axes))
         self.g.assign(kernel_norm)
 
     def _data_dep_init(self, inputs):
         """Data dependent initialization."""
         # Normalize kernel first so that calling the layer calculates
         # `tf.dot(v, x)/tf.norm(v)` as in (5) in ([Salimans and Kingma, 2016][1]).
         self._compute_weights()
@@ -132,23 +135,21 @@
         Raises
         ------
         ValueError
             If `Layer` does not contain a `kernel` of weights.
         """
         input_shape = tf.TensorShape(input_shape).as_list()
         input_shape[0] = None
-        self.input_spec = tf.keras.layers.InputSpec(shape=input_shape)
+        self.input_spec = keras.layers.InputSpec(shape=input_shape)
 
         if not self.layer.built:
             self.layer.build(input_shape)
 
             if not hasattr(self.layer, "kernel"):
-                raise ValueError(
-                    "`WeightNorm` must wrap a layer that contains a `kernel` for weights"
-                )
+                raise ValueError("`WeightNorm` must wrap a layer that contains a `kernel` for weights")
 
             self.kernel_norm_axes = list(range(self.layer.kernel.shape.ndims))
             self.kernel_norm_axes.pop(self.filter_axis)
 
             self.v = self.layer.kernel
 
             # to avoid a duplicate `kernel` variable after `build` is called
@@ -156,20 +157,18 @@
             self.g = self.add_weight(
                 name="g",
                 shape=(int(self.v.shape[self.filter_axis]),),
                 initializer="ones",
                 dtype=self.v.dtype,
                 trainable=True,
             )
-            self.initialized = self.add_weight(
-                name="initialized", dtype=tf.bool, trainable=False
-            )
+            self.initialized = self.add_weight(name="initialized", dtype=tf.bool, trainable=False)
             self.initialized.assign(False)
 
-        super(WeightNorm, self).build()
+        super().build()
 
     @tf.function
     def call(self, inputs):
         """Call `Layer`."""
         if not self.initialized:
             if self.data_init:
                 self._data_dep_init(inputs)
@@ -198,18 +197,16 @@
         validate_args
             Python `bool` indicating whether arguments should be checked for correctness.
         name
             Python `str` name given to ops managed by this object.
         """
         with tf.name_scope(name) as name:
             dtype = dtype_util.common_dtype([shift], dtype_hint=tf.float32)
-            self._shift = tensor_util.convert_nonref_to_tensor(
-                shift, dtype=dtype, name="shift"
-            )
-            super(Shift, self).__init__(
+            self._shift = tensor_util.convert_nonref_to_tensor(shift, dtype=dtype, name="shift")
+            super().__init__(
                 forward_min_event_ndims=0,
                 is_constant_jacobian=True,
                 dtype=dtype,
                 validate_args=validate_args,
                 name=name,
             )
 
@@ -232,18 +229,60 @@
         # is_constant_jacobian = True for this bijector, hence the
         # `log_det_jacobian` need only be specified for a single input, as this will
         # be tiled to match `event_ndims`.
         return tf.zeros([], dtype=dtype_util.base_dtype(x.dtype))
 
 
 class PixelCNN(distribution.Distribution):
+    """
+    Construct Pixel CNN++ distribution.
+
+    Parameters
+    ----------
+    image_shape
+        3D `TensorShape` or tuple for the `[height, width, channels]` dimensions of the image.
+    conditional_shape
+        `TensorShape` or tuple for the shape of the conditional input, or `None` if there is no conditional input.
+    num_resnet
+        The number of layers (shown in Figure 2 of [2]) within each highest-level block of Figure 2 of [1].
+    num_hierarchies
+        The number of highest-level blocks (separated by expansions/contractions of dimensions in Figure 2 of [1].)
+    num_filters
+        The number of convolutional filters.
+    num_logistic_mix
+        Number of components in the logistic mixture distribution.
+    receptive_field_dims
+        Height and width in pixels of the receptive field of the convolutional layers above and to the left
+        of a given pixel. The width (second element of the tuple) should be odd. Figure 1 (middle) of [2]
+        shows a receptive field of (3, 5) (the row containing the current pixel is included in the height).
+        The default of (3, 3) was used to produce the results in [1].
+    dropout_p
+        The dropout probability. Should be between 0 and 1.
+    resnet_activation
+        The type of activation to use in the resnet blocks. May be 'concat_elu', 'elu', or 'relu'.
+    l2_weight
+        The L2 regularization weight.
+    use_weight_norm
+        If `True` then use weight normalization (works only in Eager mode).
+    use_data_init
+        If `True` then use data-dependent initialization (has no effect if `use_weight_norm` is `False`).
+    high
+        The maximum value of the input data (255 for an 8-bit image).
+    low
+        The minimum value of the input data.
+    dtype
+        Data type of the `Distribution`.
+    name
+        The name of the `Distribution`.
+    """
+
     def __init__(
         self,
         image_shape: tuple,
-        conditional_shape: tuple = None,
+        conditional_shape: Optional[tuple] = None,
         num_resnet: int = 5,
         num_hierarchies: int = 3,
         num_filters: int = 160,
         num_logistic_mix: int = 10,
         receptive_field_dims: tuple = (3, 3),
         dropout_p: float = 0.5,
         resnet_activation: str = "concat_elu",
@@ -251,78 +290,33 @@
         use_weight_norm: bool = True,
         use_data_init: bool = True,
         high: int = 255,
         low: int = 0,
         dtype=tf.float32,
         name: str = "PixelCNN",
     ) -> None:
-        """
-        Construct Pixel CNN++ distribution.
-
-        Parameters
-        ----------
-        image_shape
-            3D `TensorShape` or tuple for the `[height, width, channels]` dimensions of the image.
-        conditional_shape
-            `TensorShape` or tuple for the shape of the conditional input, or `None` if there is no conditional input.
-        num_resnet
-            The number of layers (shown in Figure 2 of [2]) within each highest-level block of Figure 2 of [1].
-        num_hierarchies
-            The number of highest-level blocks (separated by expansions/contractions of dimensions in Figure 2 of [1].)
-        num_filters
-            The number of convolutional filters.
-        num_logistic_mix
-            Number of components in the logistic mixture distribution.
-        receptive_field_dims
-            Height and width in pixels of the receptive field of the convolutional layers above and to the left
-            of a given pixel. The width (second element of the tuple) should be odd. Figure 1 (middle) of [2]
-            shows a receptive field of (3, 5) (the row containing the current pixel is included in the height).
-            The default of (3, 3) was used to produce the results in [1].
-        dropout_p
-            The dropout probability. Should be between 0 and 1.
-        resnet_activation
-            The type of activation to use in the resnet blocks. May be 'concat_elu', 'elu', or 'relu'.
-        l2_weight
-            The L2 regularization weight.
-        use_weight_norm
-            If `True` then use weight normalization (works only in Eager mode).
-        use_data_init
-            If `True` then use data-dependent initialization (has no effect if `use_weight_norm` is `False`).
-        high
-            The maximum value of the input data (255 for an 8-bit image).
-        low
-            The minimum value of the input data.
-        dtype
-            Data type of the `Distribution`.
-        name
-            The name of the `Distribution`.
-        """
         parameters = dict(locals())
         with tf.name_scope(name) as name:
-            super(PixelCNN, self).__init__(
+            super().__init__(
                 dtype=dtype,
                 reparameterization_type=reparameterization.NOT_REPARAMETERIZED,
                 validate_args=False,
                 allow_nan_stats=True,
                 parameters=parameters,
                 name=name,
             )
 
             if not tensorshape_util.is_fully_defined(image_shape):
                 raise ValueError("`image_shape` must be fully defined.")
 
-            if conditional_shape is not None and not tensorshape_util.is_fully_defined(
-                conditional_shape
-            ):
+            if conditional_shape is not None and not tensorshape_util.is_fully_defined(conditional_shape):
                 raise ValueError("`conditional_shape` must be fully defined.")
 
             if tensorshape_util.rank(image_shape) != 3:
-                raise ValueError(
-                    "`image_shape` must have length 3, representing [height, width, channels] dimensions."
-                )
+                raise ValueError("`image_shape` must have length 3, representing [height, width, channels] dimensions.")
 
             self._high = tf.cast(high, self.dtype)
             self._low = tf.cast(low, self.dtype)
             self._num_logistic_mix = num_logistic_mix
             self.network = _PixelCNNNetwork(
                 dropout_p=dropout_p,
                 num_resnet=num_resnet,
@@ -337,26 +331,22 @@
                 dtype=dtype,
             )
 
             image_input_shape = tensorshape_util.concatenate([None], image_shape)
             if conditional_shape is None:
                 input_shape = image_input_shape
             else:
-                conditional_input_shape = tensorshape_util.concatenate(
-                    [None], conditional_shape
-                )
+                conditional_input_shape = tensorshape_util.concatenate([None], conditional_shape)
                 input_shape = [image_input_shape, conditional_input_shape]
 
             self.image_shape = image_shape
             self.conditional_shape = conditional_shape
             self.network.build(input_shape)
 
-    def _make_mixture_dist(
-        self, component_logits, locs, scales, return_per_feature: bool = False
-    ):
+    def _make_mixture_dist(self, component_logits, locs, scales, return_per_feature: bool = False):
         """Builds a mixture of quantized logistic distributions.
 
         Parameters
         ----------
         component_logits
             4D `Tensor` of logits for the Categorical distribution
             over Quantized Logistic mixture components. Dimensions are `[batch_size,
@@ -391,26 +381,22 @@
             low=self._low,
             high=self._high,
         )
 
         # mixture with logistics for the loc and scale on each pixel for each component
         dist = mixture_same_family.MixtureSameFamily(
             mixture_distribution=mixture_distribution,
-            components_distribution=independent.Independent(
-                logistic_dist, reinterpreted_batch_ndims=1
-            ),
+            components_distribution=independent.Independent(logistic_dist, reinterpreted_batch_ndims=1),
         )
         if return_per_feature:
             return dist
         else:
             return independent.Independent(dist, reinterpreted_batch_ndims=2)
 
-    def _log_prob(
-        self, value, conditional_input=None, training=None, return_per_feature=False
-    ):
+    def _log_prob(self, value, conditional_input=None, training=None, return_per_feature=False):
         """Log probability function with optional conditional input.
 
         Calculates the log probability of a batch of data under the modeled
         distribution (or conditional distribution, if conditional input is
         provided).
 
         Parameters
@@ -422,15 +408,15 @@
         conditional_input
             `Tensor` on which to condition the distribution (e.g.
             class labels), or `None`. May have leading batch dimension(s), which
             must broadcast to the leading batch dimensions of `value`.
         training
             `bool` or `None`. If `bool`, it controls the dropout layer,
             where `True` implies dropout is active. If `None`, it defaults to
-            `tf.keras.backend.learning_phase()`.
+            `keras.backend.learning_phase()`.
         return_per_feature
             `bool`. If True, return per pixel level log prob.
 
         Returns
         -------
         log_prob_values: `Tensor`.
         """
@@ -439,51 +425,41 @@
 
         # Broadcast `value` and `conditional_input` to the same batch_shape
         if conditional_input is None:
             image_batch_and_conditional_shape = image_batch_shape
         else:
             conditional_input = tf.convert_to_tensor(conditional_input)
             conditional_input_shape = prefer_static.shape(conditional_input)
-            conditional_batch_rank = prefer_static.rank(
-                conditional_input
-            ) - tensorshape_util.rank(self.conditional_shape)
+            conditional_batch_rank = prefer_static.rank(conditional_input) - tensorshape_util.rank(
+                self.conditional_shape
+            )
             conditional_batch_shape = conditional_input_shape[:conditional_batch_rank]
 
             image_batch_and_conditional_shape = prefer_static.broadcast_shape(
                 image_batch_shape, conditional_batch_shape
             )
             conditional_input = tf.broadcast_to(
                 conditional_input,
-                prefer_static.concat(
-                    [image_batch_and_conditional_shape, self.conditional_shape], axis=0
-                ),
+                prefer_static.concat([image_batch_and_conditional_shape, self.conditional_shape], axis=0),
             )
             value = tf.broadcast_to(
                 value,
-                prefer_static.concat(
-                    [image_batch_and_conditional_shape, self.event_shape], axis=0
-                ),
+                prefer_static.concat([image_batch_and_conditional_shape, self.event_shape], axis=0),
             )
 
             # Flatten batch dimension for input to Keras model
             conditional_input = tf.reshape(
                 conditional_input,
                 prefer_static.concat([(-1,), self.conditional_shape], axis=0),
             )
 
-        value = tf.reshape(
-            value, prefer_static.concat([(-1,), self.event_shape], axis=0)
-        )
+        value = tf.reshape(value, prefer_static.concat([(-1,), self.event_shape], axis=0))
 
         transformed_value = (2.0 * (value - self._low) / (self._high - self._low)) - 1.0
-        inputs = (
-            transformed_value
-            if conditional_input is None
-            else [transformed_value, conditional_input]
-        )
+        inputs = transformed_value if conditional_input is None else [transformed_value, conditional_input]
 
         params = self.network(inputs, training=training)
 
         num_channels = self.event_shape[-1]
         if num_channels == 1:
             component_logits, locs, scales = params
         else:
@@ -507,17 +483,15 @@
             for i in range(num_channels):
                 channel_tensors[i] = channel_tensors[i][..., tf.newaxis, :]
                 for j in range(i):
                     loc_tensors[i] += channel_tensors[j] * coef_tensors[coef_count]
                     coef_count += 1
             locs = tf.concat(loc_tensors, axis=-1)
 
-        dist = self._make_mixture_dist(
-            component_logits, locs, scales, return_per_feature=return_per_feature
-        )
+        dist = self._make_mixture_dist(component_logits, locs, scales, return_per_feature=return_per_feature)
         log_px = dist.log_prob(value)
         if return_per_feature:
             return log_px
         else:
             return tf.reshape(log_px, image_batch_and_conditional_shape)
 
     def _sample_n(self, n, seed=None, conditional_input=None, training=False):
@@ -540,38 +514,30 @@
 
         Returns
         -------
         samples
             a `Tensor` of shape `[n, height, width, num_channels]`.
         """
         if conditional_input is not None:
-            conditional_input = tf.convert_to_tensor(
-                conditional_input, dtype=self.dtype
-            )
+            conditional_input = tf.convert_to_tensor(conditional_input, dtype=self.dtype)
             conditional_event_rank = tensorshape_util.rank(self.conditional_shape)
             conditional_input_shape = prefer_static.shape(conditional_input)
-            conditional_sample_rank = (
-                prefer_static.rank(conditional_input) - conditional_event_rank
-            )
+            conditional_sample_rank = prefer_static.rank(conditional_input) - conditional_event_rank
 
             # If `conditional_input` has no sample dimensions, prepend a sample
             # dimension
             if conditional_sample_rank == 0:
                 conditional_input = conditional_input[tf.newaxis, ...]
                 conditional_sample_rank = 1
 
             # Assert that the conditional event shape in the `PixelCnnNetwork` is the
             # same as that implied by `conditional_input`.
             conditional_event_shape = conditional_input_shape[conditional_sample_rank:]
-            with tf.control_dependencies(
-                [tf.assert_equal(self.conditional_shape, conditional_event_shape)]
-            ):
-                conditional_sample_shape = conditional_input_shape[
-                    :conditional_sample_rank
-                ]
+            with tf.control_dependencies([tf.assert_equal(self.conditional_shape, conditional_event_shape)]):
+                conditional_sample_shape = conditional_input_shape[:conditional_sample_rank]
                 repeat = n // prefer_static.reduce_prod(conditional_sample_shape)
                 h = tf.reshape(
                     conditional_input,
                     prefer_static.concat([(-1,), self.conditional_shape], axis=0),
                 )
                 h = tf.tile(
                     h,
@@ -630,21 +596,17 @@
 
         index0 = tf.zeros([], dtype=tf.int32)
 
         # Construct the while loop for sampling
         total_pixels = image_height * image_width
         loop_cond = lambda ind, _: tf.less(ind, total_pixels)  # noqa: E731
         init_vars = (index0, samples_0)
-        _, samples = tf.while_loop(
-            loop_cond, loop_body, init_vars, parallel_iterations=1
-        )
+        _, samples = tf.while_loop(loop_cond, loop_body, init_vars, parallel_iterations=1)
 
-        transformed_samples = self._low + 0.5 * (self._high - self._low) * (
-            samples + 1.0
-        )
+        transformed_samples = self._low + 0.5 * (self._high - self._low) * (samples + 1.0)
         return tf.round(transformed_samples)
 
     def _sample_channels(self, component_logits, locs, scales, coeffs=None, seed=None):
         """Sample a single pixel-iteration and apply channel conditioning.
 
         Parameters
         ----------
@@ -674,17 +636,15 @@
             4D `Tensor` of sampled image data with autoregression among \
             channels. Dimensions are `[batch_size, height, width, num_channels]`.
         """
         num_channels = self.event_shape[-1]
 
         # sample mixture components once for the entire pixel
         component_dist = categorical.Categorical(logits=component_logits)
-        mask = tf.one_hot(
-            indices=component_dist.sample(seed=seed), depth=self._num_logistic_mix
-        )
+        mask = tf.one_hot(indices=component_dist.sample(seed=seed), depth=self._num_logistic_mix)
         mask = tf.cast(mask[..., tf.newaxis], self.dtype)
 
         # apply mixture component mask and separate out RGB parameters
         masked_locs = tf.reduce_sum(locs * mask, axis=-2)
         loc_tensors = tf.split(masked_locs, num_channels, axis=-1)
         masked_scales = tf.reduce_sum(scales * mask, axis=-2)
         scale_tensors = tf.split(masked_scales, num_channels, axis=-1)
@@ -698,30 +658,28 @@
         coef_count = 0
         for i in range(num_channels):
             loc = loc_tensors[i]
             for c in channel_samples:
                 loc += c * coef_tensors[coef_count]
                 coef_count += 1
 
-            logistic_samp = logistic.Logistic(loc=loc, scale=scale_tensors[i]).sample(
-                seed=seed
-            )
+            logistic_samp = logistic.Logistic(loc=loc, scale=scale_tensors[i]).sample(seed=seed)
             logistic_samp = tf.clip_by_value(logistic_samp, -1.0, 1.0)
             channel_samples.append(logistic_samp)
 
         return tf.concat(channel_samples, axis=-1)
 
     def _batch_shape(self):
         return tf.TensorShape([])
 
     def _event_shape(self):
         return tf.TensorShape(self.image_shape)
 
 
-class _PixelCNNNetwork(tf.keras.layers.Layer):
+class _PixelCNNNetwork(keras.layers.Layer):
     """Keras `Layer` to parameterize a Pixel CNN++ distribution.
     This is a Keras implementation of the Pixel CNN++ network, as described in
     Salimans et al. (2017)[1] and van den Oord et al. (2016)[2].
     (https://github.com/openai/pixel-cnn).
     #### References
     [1]: Tim Salimans, Andrej Karpathy, Xi Chen, and Diederik P. Kingma.
        PixelCNN++: Improving the PixelCNN with Discretized Logistic Mixture
@@ -783,23 +741,21 @@
             `bool`, if `True` then use weight normalization.
         use_data_init
             `bool`, if `True` then use data-dependent initialization
             (has no effect if `use_weight_norm` is `False`).
         dtype
             Data type of the layer.
         """
-        super(_PixelCNNNetwork, self).__init__(dtype=dtype)
+        super().__init__(dtype=dtype)
         self._dropout_p = dropout_p
         self._num_resnet = num_resnet
         self._num_hierarchies = num_hierarchies
         self._num_filters = num_filters
         self._num_logistic_mix = num_logistic_mix
-        self._receptive_field_dims = (
-            receptive_field_dims  # first set desired receptive field, then infer kernel
-        )
+        self._receptive_field_dims = receptive_field_dims  # first set desired receptive field, then infer kernel
         self._resnet_activation = resnet_activation
         self._l2_weight = l2_weight
 
         if use_weight_norm:
 
             def layer_wrapper(layer):
                 def wrapped_layer(*args, **kwargs):
@@ -811,52 +767,48 @@
         else:
             self._layer_wrapper = lambda layer: layer
 
     def build(self, input_shape):
         dtype = self.dtype
         if len(input_shape) == 2:
             batch_image_shape, batch_conditional_shape = input_shape
-            conditional_input = tf.keras.layers.Input(
-                shape=batch_conditional_shape[1:], dtype=dtype
-            )
+            conditional_input = keras.layers.Input(shape=batch_conditional_shape[1:], dtype=dtype)
         else:
             batch_image_shape = input_shape
             conditional_input = None
 
         image_shape = batch_image_shape[1:]
-        image_input = tf.keras.layers.Input(shape=image_shape, dtype=dtype)
+        image_input = keras.layers.Input(shape=image_shape, dtype=dtype)
 
         if self._resnet_activation == "concat_elu":
-            activation = tf.keras.layers.Lambda(
-                lambda x: tf.nn.elu(tf.concat([x, -x], axis=-1)), dtype=dtype
-            )
+            activation = keras.layers.Lambda(lambda x: tf.nn.elu(tf.concat([x, -x], axis=-1)), dtype=dtype)
         else:
-            activation = tf.keras.activations.get(self._resnet_activation)
+            activation = keras.activations.get(self._resnet_activation)
 
         # Define layers with default inputs and layer wrapper applied
         Conv2D = functools.partial(  # pylint:disable=invalid-name
-            self._layer_wrapper(tf.keras.layers.Convolution2D),
+            self._layer_wrapper(keras.layers.Convolution2D),
             filters=self._num_filters,
             padding="same",
-            kernel_regularizer=tf.keras.regularizers.l2(self._l2_weight),
+            kernel_regularizer=keras.regularizers.l2(self._l2_weight),
             dtype=dtype,
         )
 
         Dense = functools.partial(  # pylint:disable=invalid-name
-            self._layer_wrapper(tf.keras.layers.Dense),
-            kernel_regularizer=tf.keras.regularizers.l2(self._l2_weight),
+            self._layer_wrapper(keras.layers.Dense),
+            kernel_regularizer=keras.regularizers.l2(self._l2_weight),
             dtype=dtype,
         )
 
         Conv2DTranspose = functools.partial(  # pylint:disable=invalid-name
-            self._layer_wrapper(tf.keras.layers.Conv2DTranspose),
+            self._layer_wrapper(keras.layers.Conv2DTranspose),
             filters=self._num_filters,
             padding="same",
             strides=(2, 2),
-            kernel_regularizer=tf.keras.regularizers.l2(self._l2_weight),
+            kernel_regularizer=keras.regularizers.l2(self._l2_weight),
             dtype=dtype,
         )
 
         rows, cols = self._receptive_field_dims
 
         # Define the dimensions of the valid (unmasked) areas of the layer kernels
         # for stride 1 convolutions in the internal layers.
@@ -868,48 +820,41 @@
         # Define the size of the kernel necessary to center the current pixel
         # correctly for stride 1 convolutions in the internal layers.
         kernel_sizes = {"vertical": (2 * rows - 3, cols), "horizontal": (3, cols)}
 
         # Make the kernel constraint functions for stride 1 convolutions in internal
         # layers.
         kernel_constraints = {
-            k: _make_kernel_constraint(kernel_sizes[k], (0, v[0]), (0, v[1]))
-            for k, v in kernel_valid_dims.items()
+            k: _make_kernel_constraint(kernel_sizes[k], (0, v[0]), (0, v[1])) for k, v in kernel_valid_dims.items()
         }
 
         # Build the initial vertical stack/horizontal stack convolutional layers,
         # as shown in Figure 1 of [2]. The receptive field of the initial vertical
         # stack layer is a rectangular area centered above the current pixel.
         vertical_stack_init = Conv2D(
             kernel_size=(2 * rows - 1, cols),
-            kernel_constraint=_make_kernel_constraint(
-                (2 * rows - 1, cols), (0, rows - 1), (0, cols)
-            ),
+            kernel_constraint=_make_kernel_constraint((2 * rows - 1, cols), (0, rows - 1), (0, cols)),
         )(image_input)
 
         # In Figure 1 [2], the receptive field of the horizontal stack is
         # illustrated as the pixels in the same row and to the left of the current
         # pixel. [1] increases the height of this receptive field from one pixel to
         # two (`horizontal_stack_left`) and additionally includes a subset of the
         # row of pixels centered above the current pixel (`horizontal_stack_up`).
         horizontal_stack_up = Conv2D(
             kernel_size=(3, cols),
             kernel_constraint=_make_kernel_constraint((3, cols), (0, 1), (0, cols)),
         )(image_input)
 
         horizontal_stack_left = Conv2D(
             kernel_size=(3, cols),
-            kernel_constraint=_make_kernel_constraint(
-                (3, cols), (0, 2), (0, cols // 2)
-            ),
+            kernel_constraint=_make_kernel_constraint((3, cols), (0, 2), (0, cols // 2)),
         )(image_input)
 
-        horizontal_stack_init = tf.keras.layers.add(
-            [horizontal_stack_up, horizontal_stack_left], dtype=dtype
-        )
+        horizontal_stack_init = keras.layers.add([horizontal_stack_up, horizontal_stack_left], dtype=dtype)
 
         layer_stacks = {
             "vertical": [vertical_stack_init],
             "horizontal": [horizontal_stack_init],
         }
 
         # Build the downward pass of the U-net (left-hand half of Figure 2 of [1]).
@@ -933,54 +878,46 @@
                         kernel_constraint=kernel_constraints[stack],
                     )(x)
 
                     # Add the vertical-stack layer to the horizontal-stack layer
                     if stack == "horizontal":
                         h = activation(layer_stacks["vertical"][-1])
                         h = Dense(self._num_filters)(h)
-                        x = tf.keras.layers.add([h, x], dtype=dtype)
+                        x = keras.layers.add([h, x], dtype=dtype)
 
                     x = activation(x)
-                    x = tf.keras.layers.Dropout(self._dropout_p, dtype=dtype)(x)
+                    x = keras.layers.Dropout(self._dropout_p, dtype=dtype)(x)
                     x = Conv2D(
                         filters=2 * self._num_filters,
                         kernel_size=kernel_sizes[stack],
                         kernel_constraint=kernel_constraints[stack],
                     )(x)
 
                     if conditional_input is not None:
-                        h_projection = _build_and_apply_h_projection(
-                            conditional_input, self._num_filters, dtype=dtype
-                        )
-                        x = tf.keras.layers.add([x, h_projection], dtype=dtype)
+                        h_projection = _build_and_apply_h_projection(conditional_input, self._num_filters, dtype=dtype)
+                        x = keras.layers.add([x, h_projection], dtype=dtype)
 
                     x = _apply_sigmoid_gating(x)
 
                     # Add a residual connection from the layer's input.
-                    out = tf.keras.layers.add([input_x, x], dtype=dtype)
+                    out = keras.layers.add([input_x, x], dtype=dtype)
                     layer_stacks[stack].append(out)
 
             if i < self._num_hierarchies - 1:
                 # Build convolutional layers that contract the height/width dimensions
                 # on the downward pass between each set of layers (e.g. contracting from
                 # 32x32 to 16x16 in Figure 2 of [1]).
                 for stack in ["vertical", "horizontal"]:
                     # Define kernel dimensions/masking to maintain the autoregressive property.
                     x = layer_stacks[stack][-1]
                     h, w = kernel_valid_dims[stack]
                     kernel_height = 2 * h
-                    if stack == "vertical":
-                        kernel_width = w + 1
-                    else:
-                        kernel_width = 2 * w
-
+                    kernel_width = w + 1 if stack == "vertical" else 2 * w
                     kernel_size = (kernel_height, kernel_width)
-                    kernel_constraint = _make_kernel_constraint(
-                        kernel_size, (0, h), (0, w)
-                    )
+                    kernel_constraint = _make_kernel_constraint(kernel_size, (0, h), (0, w))
                     x = Conv2D(
                         strides=(2, 2),
                         kernel_size=kernel_size,
                         kernel_constraint=kernel_constraint,
                     )(x)
                     layer_stacks[stack].append(x)
 
@@ -1010,40 +947,38 @@
                         kernel_size=kernel_sizes[stack],
                         kernel_constraint=kernel_constraints[stack],
                     )(x)
 
                     # Include the vertical-stack layer of the upward pass in the layers
                     # to be added to the horizontal layer.
                     if stack == "horizontal":
-                        x_symmetric = tf.keras.layers.Concatenate(axis=-1, dtype=dtype)(
+                        x_symmetric = keras.layers.Concatenate(axis=-1, dtype=dtype)(
                             [upward_pass["vertical"], x_symmetric]
                         )
 
                     # Add a skip-connection from the symmetric layer in the downward
                     # pass to the layer `x` in the upward pass.
                     h = activation(x_symmetric)
                     h = Dense(self._num_filters)(h)
-                    x = tf.keras.layers.add([h, x], dtype=dtype)
+                    x = keras.layers.add([h, x], dtype=dtype)
 
                     x = activation(x)
-                    x = tf.keras.layers.Dropout(self._dropout_p, dtype=dtype)(x)
+                    x = keras.layers.Dropout(self._dropout_p, dtype=dtype)(x)
                     x = Conv2D(
                         filters=2 * self._num_filters,
                         kernel_size=kernel_sizes[stack],
                         kernel_constraint=kernel_constraints[stack],
                     )(x)
 
                     if conditional_input is not None:
-                        h_projection = _build_and_apply_h_projection(
-                            conditional_input, self._num_filters, dtype=dtype
-                        )
-                        x = tf.keras.layers.add([x, h_projection], dtype=dtype)
+                        h_projection = _build_and_apply_h_projection(conditional_input, self._num_filters, dtype=dtype)
+                        x = keras.layers.add([x, h_projection], dtype=dtype)
 
                     x = _apply_sigmoid_gating(x)
-                    upward_pass[stack] = tf.keras.layers.add([input_x, x], dtype=dtype)
+                    upward_pass[stack] = keras.layers.add([input_x, x], dtype=dtype)
 
             # Define deconvolutional layers that expand height/width dimensions on the
             # upward pass (e.g. expanding from 8x8 to 16x16 in Figure 2 of [1]), with
             # the correct kernel dimensions/masking to maintain the autoregressive
             # property.
             if i < self._num_hierarchies - 1:
                 for stack in ["vertical", "horizontal"]:
@@ -1067,25 +1002,21 @@
                     x = upward_pass[stack]
                     x = Conv2DTranspose(
                         kernel_size=(kernel_height, kernel_width),
                         kernel_constraint=kernel_constraint,
                     )(x)
                     upward_pass[stack] = x
 
-        x_out = tf.keras.layers.ELU(dtype=dtype)(upward_pass["horizontal"])
+        x_out = keras.layers.ELU(dtype=dtype)(upward_pass["horizontal"])
 
         # Build final Dense/Reshape layers to output the correct number of
         # parameters per pixel.
         num_channels = tensorshape_util.as_list(image_shape)[-1]
-        num_coeffs = (
-            num_channels * (num_channels - 1) // 2
-        )  # alpha, beta, gamma in eq.3 of paper
-        num_out = (
-            num_channels * 2 + num_coeffs + 1
-        )  # mu, s + alpha, beta, gamma + 1 (mixture weight)
+        num_coeffs = num_channels * (num_channels - 1) // 2  # alpha, beta, gamma in eq.3 of paper
+        num_out = num_channels * 2 + num_coeffs + 1  # mu, s + alpha, beta, gamma + 1 (mixture weight)
         num_out_total = num_out * self._num_logistic_mix
         params = Dense(num_out_total)(x_out)
         params = tf.reshape(
             params,
             prefer_static.concat(  # [-1,H,W,nb mixtures, params per mixture]
                 [[-1], image_shape[:-1], [self._num_logistic_mix, num_out]], axis=0
             ),
@@ -1103,21 +1034,17 @@
 
         # Squeeze singleton dimension from component logits
         outputs[0] = tf.squeeze(outputs[0], axis=-1)
 
         # Ensure scales are positive and do not collapse to near-zero
         outputs[2] = tf.nn.softplus(outputs[2]) + tf.cast(tf.exp(-7.0), self.dtype)
 
-        inputs = (
-            image_input
-            if conditional_input is None
-            else [image_input, conditional_input]
-        )
-        self._network = tf.keras.Model(inputs=inputs, outputs=outputs)
-        super(_PixelCNNNetwork, self).build(input_shape)
+        inputs = image_input if conditional_input is None else [image_input, conditional_input]
+        self._network = keras.Model(inputs=inputs, outputs=outputs)
+        super().build(input_shape)
 
     def call(self, inputs, training=None):
         """Call the Pixel CNN network model.
 
         Parameters
         ----------
         inputs
@@ -1125,15 +1052,15 @@
             width, channels] or a 2-element `list`. If `list`, the first element is
             the 4D image `Tensor` and the second element is a `Tensor` with
             conditional input data (e.g. VAE encodings or class labels) with the
             same leading batch dimension as the image `Tensor`.
         training
             `bool` or `None`. If `bool`, it controls the dropout layer,
             where `True` implies dropout is active. If `None`, it it defaults to
-            `tf.keras.backend.learning_phase()`
+            `keras.backend.learning_phase()`
 
         Returns
         -------
         outputs
             a 3- or 4-element `list` of `Tensor`s in the following order: \
             component_logits: 4D `Tensor` of logits for the Categorical distribution \
             over Quantized Logistic mixture components. Dimensions are \
@@ -1163,19 +1090,17 @@
     mask[lower:upper, left:right] = 1.0
     mask = mask[:, :, np.newaxis, np.newaxis]
     return lambda x: x * mask
 
 
 def _build_and_apply_h_projection(h, num_filters, dtype):
     """Project the conditional input."""
-    h = tf.keras.layers.Flatten(dtype=dtype)(h)
-    h_projection = tf.keras.layers.Dense(
-        2 * num_filters, kernel_initializer="random_normal", dtype=dtype
-    )(h)
+    h = keras.layers.Flatten(dtype=dtype)(h)
+    h_projection = keras.layers.Dense(2 * num_filters, kernel_initializer="random_normal", dtype=dtype)(h)
     return h_projection[..., tf.newaxis, tf.newaxis, :]
 
 
 def _apply_sigmoid_gating(x):
     """Apply the sigmoid gating in Figure 2 of [2]."""
     activation_tensor, gate_tensor = tf.split(x, 2, axis=-1)
     sigmoid_gate = tf.sigmoid(gate_tensor)
-    return tf.keras.layers.multiply([sigmoid_gate, activation_tensor], dtype=x.dtype)
+    return keras.layers.multiply([sigmoid_gate, activation_tensor], dtype=x.dtype)
```

### Comparing `daml-0.51.0/src/daml/_internal/metrics/base.py` & `daml-0.52.0/src/daml/_internal/metrics/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,11 +73,9 @@
     def method(self, value: TMethods):
         self._set_method(value)
 
     def _set_method(self, value: TMethods):
         """This setter is to fix pyright incorrect detection of
         incorrectly overriding the 'method' property"""
         if value not in self.methods():
-            raise KeyError(
-                f"Specified method not available for class ({self.methods()})."
-            )
+            raise KeyError(f"Specified method not available for class ({self.methods()}).")
         self._method_key = value
```

### Comparing `daml-0.51.0/src/daml/_internal/metrics/ber.py` & `daml-0.52.0/src/daml/_internal/metrics/ber.py`

 * *Files identical despite different names*

### Comparing `daml-0.51.0/src/daml/_internal/metrics/divergence.py` & `daml-0.52.0/src/daml/_internal/metrics/divergence.py`

 * *Files identical despite different names*

### Comparing `daml-0.51.0/src/daml/_internal/metrics/drift/base.py` & `daml-0.52.0/src/daml/_internal/metrics/drift/base.py`

 * *Files identical despite different names*

### Comparing `daml-0.51.0/src/daml/_internal/metrics/drift/cvm.py` & `daml-0.52.0/src/daml/_internal/metrics/drift/cvm.py`

 * *Files identical despite different names*

### Comparing `daml-0.51.0/src/daml/_internal/metrics/drift/ks.py` & `daml-0.52.0/src/daml/_internal/metrics/drift/ks.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,11 +92,9 @@
         Feature level p-values and K-S statistics.
         """
         x = x.reshape(x.shape[0], -1)
         x_ref = self.x_ref.reshape(self.x_ref.shape[0], -1)
         p_val = np.zeros(self.n_features, dtype=np.float32)
         dist = np.zeros_like(p_val)
         for f in range(self.n_features):
-            dist[f], p_val[f] = ks_2samp(
-                x_ref[:, f], x[:, f], alternative=self.alternative, method="exact"
-            )
+            dist[f], p_val[f] = ks_2samp(x_ref[:, f], x[:, f], alternative=self.alternative, method="exact")
         return p_val, dist
```

### Comparing `daml-0.51.0/src/daml/_internal/metrics/drift/mmd.py` & `daml-0.52.0/src/daml/_internal/metrics/drift/mmd.py`

 * *Files 5% similar despite different names*

```diff
@@ -72,51 +72,37 @@
     ) -> None:
         super().__init__(x_ref, p_val, x_ref_preprocessed, update_x_ref, preprocess_fn)
 
         self.infer_sigma = configure_kernel_from_x_ref
         if configure_kernel_from_x_ref and isinstance(sigma, np.ndarray):
             self.infer_sigma = False
 
-        self.n_permutations = (
-            n_permutations  # nb of iterations through permutation test
-        )
+        self.n_permutations = n_permutations  # nb of iterations through permutation test
 
         # set device
         self.device = get_device(device)
 
         # initialize kernel
-        sigma_tensor = (
-            torch.from_numpy(sigma).to(self.device)
-            if isinstance(sigma, np.ndarray)
-            else None
-        )
-        self.kernel = (
-            kernel(sigma_tensor).to(self.device) if kernel == GaussianRBF else kernel
-        )
+        sigma_tensor = torch.from_numpy(sigma).to(self.device) if isinstance(sigma, np.ndarray) else None
+        self.kernel = kernel(sigma_tensor).to(self.device) if kernel == GaussianRBF else kernel
 
         # compute kernel matrix for the reference data
         if self.infer_sigma or isinstance(sigma_tensor, torch.Tensor):
             x = torch.from_numpy(self.x_ref).to(self.device)
             self.k_xx = self.kernel(x, x, infer_sigma=self.infer_sigma)
             self.infer_sigma = False
         else:
             self.k_xx, self.infer_sigma = None, True
 
     def _kernel_matrix(self, x: torch.Tensor, y: torch.Tensor) -> torch.Tensor:
         """Compute and return full kernel matrix between arrays x and y."""
         k_xy = self.kernel(x, y, self.infer_sigma)
-        k_xx = (
-            self.k_xx
-            if self.k_xx is not None and self.update_x_ref is None
-            else self.kernel(x, x)
-        )
+        k_xx = self.k_xx if self.k_xx is not None and self.update_x_ref is None else self.kernel(x, x)
         k_yy = self.kernel(y, y)
-        kernel_mat = torch.cat(
-            [torch.cat([k_xx, k_xy], 1), torch.cat([k_xy.T, k_yy], 1)], 0
-        )
+        kernel_mat = torch.cat([torch.cat([k_xx, k_xy], 1), torch.cat([k_xy.T, k_yy], 1)], 0)
         return kernel_mat
 
     @preprocess_x
     def score(self, x: np.ndarray) -> Tuple[float, float, float]:
         """
         Compute the p-value resulting from a permutation test using the maximum mean
         discrepancy as a distance measure between the reference data and the data to
@@ -134,26 +120,21 @@
         """
         x_ref = torch.from_numpy(self.x_ref).to(self.device)
         n = x.shape[0]
         kernel_mat = self._kernel_matrix(x_ref, torch.from_numpy(x).to(self.device))
         kernel_mat = kernel_mat - torch.diag(kernel_mat.diag())  # zero diagonal
         mmd2 = mmd2_from_kernel_matrix(kernel_mat, n, permute=False, zero_diag=False)
         mmd2_permuted = torch.Tensor(
-            [
-                mmd2_from_kernel_matrix(kernel_mat, n, permute=True, zero_diag=False)
-                for _ in range(self.n_permutations)
-            ]
+            [mmd2_from_kernel_matrix(kernel_mat, n, permute=True, zero_diag=False) for _ in range(self.n_permutations)]
         )
         mmd2, mmd2_permuted = mmd2.cpu(), mmd2_permuted.cpu()
         p_val = (mmd2 <= mmd2_permuted).float().mean()
         # compute distance threshold
         idx_threshold = int(self.p_val * len(mmd2_permuted))
-        distance_threshold = torch.sort(mmd2_permuted, descending=True).values[
-            idx_threshold
-        ]
+        distance_threshold = torch.sort(mmd2_permuted, descending=True).values[idx_threshold]
         return p_val.numpy().item(), mmd2.numpy().item(), distance_threshold.numpy()
 
     @preprocess_x
     @update_x_ref
     def predict(
         self,
         x: np.ndarray,
```

### Comparing `daml-0.51.0/src/daml/_internal/metrics/drift/torch.py` & `daml-0.52.0/src/daml/_internal/metrics/drift/torch.py`

 * *Files 1% similar despite different names*

```diff
@@ -120,17 +120,15 @@
             preds_tmp = model(x_batch.to(device))
             if isinstance(preds_tmp, (list, tuple)):
                 if len(preds) == 0:  # init tuple with lists to store predictions
                     preds = tuple([] for _ in range(len(preds_tmp)))
                 for j, p in enumerate(preds_tmp):
                     if isinstance(p, torch.Tensor):
                         p = p.cpu()
-                    preds[j].append(
-                        p if not return_np or isinstance(p, np.ndarray) else p.numpy()
-                    )
+                    preds[j].append(p if not return_np or isinstance(p, np.ndarray) else p.numpy())
             elif isinstance(preds_tmp, (np.ndarray, torch.Tensor)):
                 if isinstance(preds_tmp, torch.Tensor):
                     preds_tmp = preds_tmp.cpu()
                 if isinstance(preds, tuple):
                     preds = list(preds)
                 preds.append(
                     preds_tmp
@@ -296,21 +294,17 @@
         infer_sigma: bool = False,
     ) -> torch.Tensor:
         x, y = torch.as_tensor(x), torch.as_tensor(y)
         dist = squared_pairwise_distance(x.flatten(1), y.flatten(1))  # [Nx, Ny]
 
         if infer_sigma or self.init_required:
             if self.trainable and infer_sigma:
-                raise ValueError(
-                    "Gradients cannot be computed w.r.t. an inferred sigma value"
-                )
+                raise ValueError("Gradients cannot be computed w.r.t. an inferred sigma value")
             sigma = self.init_sigma_fn(x, y, dist)
             with torch.no_grad():
                 self.log_sigma.copy_(sigma.log().clone())
             self.init_required = False
 
         gamma = 1.0 / (2.0 * self.sigma**2)  # [Ns,]
         # TODO: do matrix multiplication after all?
-        kernel_mat = torch.exp(
-            -torch.cat([(g * dist)[None, :, :] for g in gamma], dim=0)
-        )  # [Ns, Nx, Ny]
+        kernel_mat = torch.exp(-torch.cat([(g * dist)[None, :, :] for g in gamma], dim=0))  # [Ns, Nx, Ny]
         return kernel_mat.mean(dim=0)  # [Nx, Ny]
```

### Comparing `daml-0.51.0/src/daml/_internal/metrics/drift/uncertainty.py` & `daml-0.52.0/src/daml/_internal/metrics/drift/uncertainty.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,17 +47,15 @@
     if preds_type == "probs":
         if np.abs(1 - np.sum(preds, axis=-1)).mean() > 1e-6:
             raise ValueError("Probabilities across labels should sum to 1")
         probs = preds
     elif preds_type == "logits":
         probs = softmax(preds, axis=-1)
     else:
-        raise NotImplementedError(
-            "Only prediction types 'probs' and 'logits' supported."
-        )
+        raise NotImplementedError("Only prediction types 'probs' and 'logits' supported.")
 
     uncertainties = entropy(probs, axis=-1)
     return uncertainties[:, None]  # Detectors expect N x d  # type: ignore
 
 
 class UncertaintyDrift:
     """
```

### Comparing `daml-0.51.0/src/daml/_internal/metrics/sufficiency.py` & `daml-0.52.0/src/daml/_internal/metrics/sufficiency.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,17 +91,15 @@
     if STEPS_KEY not in data:
         raise KeyError(f"{STEPS_KEY} is a required key for Sufficiency output.")
     c = len(data[STEPS_KEY])
     for m, v in data.items():
         if m == STEPS_KEY:
             continue
         if c != len(v):
-            raise ValueError(
-                "f{m} does not contain the expected number ({c}) of data points."
-            )
+            raise ValueError("f{m} does not contain the expected number ({c}) of data points.")
 
 
 def project_steps(
     measure: np.ndarray,
     steps: np.ndarray,
     projection: np.ndarray,
 ) -> np.ndarray:
@@ -184,17 +182,15 @@
 
     def __init__(
         self,
         model: nn.Module,
         train_ds: Dataset,
         test_ds: Dataset,
         train_fn: Callable[[nn.Module, Dataset, Sequence[int]], None],
-        eval_fn: Callable[
-            [nn.Module, Dataset], Union[Dict[str, float], Dict[str, np.ndarray]]
-        ],
+        eval_fn: Callable[[nn.Module, Dataset], Union[Dict[str, float], Dict[str, np.ndarray]]],
         runs: int = 1,
         substeps: int = 5,
         train_kwargs: Optional[Dict[str, Any]] = None,
         eval_kwargs: Optional[Dict[str, Any]] = None,
     ):
         self.model = model
         self.train_ds = train_ds
@@ -239,17 +235,15 @@
         self,
     ) -> Callable[[nn.Module, Dataset], Union[Dict[str, float], Dict[str, np.ndarray]]]:
         return self._eval_fn
 
     @eval_fn.setter
     def eval_fn(
         self,
-        value: Callable[
-            [nn.Module, Dataset], Union[Dict[str, float], Dict[str, np.ndarray]]
-        ],
+        value: Callable[[nn.Module, Dataset], Union[Dict[str, float], Dict[str, np.ndarray]]],
     ):
         if not callable(value):
             raise TypeError("Must provide a callable for eval_fn.")
         self._eval_fn = value
 
     @property
     def train_kwargs(self) -> Dict[str, Any]:
@@ -311,29 +305,23 @@
 
                 # Keep track of each measures values
                 for name, value in output.items():
                     if name == STEPS_KEY:
                         raise KeyError(f"Cannot use '{STEPS_KEY}' as a metric name.")
 
                     if name not in metric_outputs:
-                        shape = (
-                            (self.substeps, len(value))
-                            if isinstance(value, np.ndarray)
-                            else self.substeps
-                        )
+                        shape = (self.substeps, len(value)) if isinstance(value, np.ndarray) else self.substeps
                         metric_outputs[name] = np.zeros(shape)
 
                     # Sum result into current substep iteration to be averaged later
                     metric_outputs[name][iteration] += value
 
         output = {STEPS_KEY: ranges}
         # The mean for each measure must be calculated before being returned
-        output.update(
-            {name: value / self.runs for name, value in metric_outputs.items()}
-        )
+        output.update({name: value / self.runs for name, value in metric_outputs.items()})
 
         return output
 
     @classmethod
     def project(
         cls,
         data: Dict[str, np.ndarray],
@@ -354,42 +342,36 @@
             If STEPS_KEY or measure is not a valid key
         ValueError
             If the length of data points in the measures do not match
             If the steps are not int, Sequence[int] or an ndarray
         """
         validate_output(data)
         projection = [projection] if isinstance(projection, int) else projection
-        projection = (
-            np.array(projection) if isinstance(projection, Sequence) else projection
-        )
+        projection = np.array(projection) if isinstance(projection, Sequence) else projection
         if not isinstance(projection, np.ndarray):
             raise ValueError("'steps' must be an int, Sequence[int] or ndarray")
 
         output = {}
         output[STEPS_KEY] = projection
         for name, measure in data.items():
             if name == STEPS_KEY:
                 continue
 
             if len(measure.shape) > 1:
                 result = []
                 for i in range(measure.shape[1]):
-                    projected = project_steps(
-                        measure[:, i], data[STEPS_KEY], projection
-                    )
+                    projected = project_steps(measure[:, i], data[STEPS_KEY], projection)
                     result.append(projected)
                 output[name] = np.array(result).T
             else:
                 output[name] = project_steps(measure, data[STEPS_KEY], projection)
         return output
 
     @classmethod
-    def plot(
-        cls, data: Dict[str, np.ndarray], class_names: Optional[Sequence[str]] = None
-    ) -> List[Figure]:
+    def plot(cls, data: Dict[str, np.ndarray], class_names: Optional[Sequence[str]] = None) -> List[Figure]:
         """Plotting function for data sufficiency tasks
 
         Parameters
         ----------
         data : Dict[str, np.ndarray]
             Dataclass containing the average of each measure per substep
```

### Comparing `daml-0.51.0/src/daml/_internal/metrics/uap.py` & `daml-0.52.0/src/daml/_internal/metrics/uap.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,11 +37,9 @@
             uap : The empirical mean precision estimate
 
         Raises
         ------
         ValueError
             If unique classes M < 2
         """
-        uap = float(
-            average_precision_score(self.labels, self.scores, average="weighted")
-        )
+        uap = float(average_precision_score(self.labels, self.scores, average="weighted"))
         return {"uap": uap}
```

### Comparing `daml-0.51.0/src/daml/_internal/metrics/utils.py` & `daml-0.52.0/src/daml/_internal/metrics/utils.py`

 * *Files identical despite different names*

### Comparing `daml-0.51.0/src/daml/_internal/models/pytorch/autoencoder.py` & `daml-0.52.0/src/daml/_internal/models/pytorch/autoencoder.py`

 * *Files 2% similar despite different names*

```diff
@@ -138,27 +138,22 @@
             Data encoded by the model
         """
         self.model.eval()
         dl = DataLoader(dataset, batch_size=self.batch_size)
         encodings = torch.Tensor([])
 
         # Get encode function if defined
-        if getattr(self.model, "encode", None) is not None:
-            encode_func = self.model.encode
-        else:
-            encode_func = self.model.forward
+        encode_func = self.model.encode if getattr(self.model, "encode", None) else self.model.forward
+
         # Accumulate encodings from batches
         for batch in dl:
             imgs = get_images_from_batch(batch)
             imgs = imgs.to(self.device)
             embeddings = encode_func(imgs).to("cpu")
-            if len(encodings):
-                encodings = torch.vstack((encodings, embeddings))
-            else:
-                encodings = embeddings
+            encodings = torch.vstack((encodings, embeddings)) if len(encodings) else embeddings
 
         return encodings
 
 
 class AriaAutoencoder(nn.Module):
     def __init__(self, channels=3):
         super().__init__()
```

### Comparing `daml-0.51.0/src/daml/_internal/models/pytorch/blocks.py` & `daml-0.52.0/src/daml/_internal/models/pytorch/blocks.py`

 * *Files identical despite different names*

### Comparing `daml-0.51.0/src/daml/_internal/models/pytorch/utils.py` & `daml-0.52.0/src/daml/_internal/models/pytorch/utils.py`

 * *Files identical despite different names*

### Comparing `daml-0.51.0/src/daml/_prototype/README.md` & `daml-0.52.0/src/daml/_prototype/README.md`

 * *Files identical despite different names*

### Comparing `daml-0.51.0/src/daml/_prototype/cleaning.py` & `daml-0.52.0/src/daml/_prototype/cleaning.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,33 +23,26 @@
         return "outlier"
     elif level >= dist_arr.shape[0] * 2 / 3:
         return "potential outlier"
     else:
         return ""
 
 
-def get_distance(
-    cluster, level, sample, distance_array, distance_matrix, sample_clusters
-):
+def get_distance(cluster, level, sample, distance_array, distance_matrix, sample_clusters):
     # Convert the condensed distance matrix to a square form
     square_distance_matrix = squareform(distance_matrix)
 
     # For each cluster, check if it is active at the current level
     for cluster_num, level_info in sample_clusters.items():
         if cluster_num != cluster and level in level_info:
             samples = level_info[level]["samples"]
 
             for other_sample in samples:
-                if (
-                    square_distance_matrix[sample, other_sample]
-                    < distance_array[cluster]
-                ):
-                    distance_array[cluster] = square_distance_matrix[
-                        sample, other_sample
-                    ]
+                if square_distance_matrix[sample, other_sample] < distance_array[cluster]:
+                    distance_array[cluster] = square_distance_matrix[sample, other_sample]
 
     return distance_array
 
 
 def reorganize_clusters(clusters):
     """
     Reorganize the clusters dictionary to be nested by cluster_num, then by level,
@@ -73,17 +66,15 @@
         # Initialize the structure if not present
         if cluster_num not in new_structure:
             new_structure[cluster_num] = {}
 
         if level not in new_structure[cluster_num] and level == 1:
             new_structure[cluster_num][level] = {"samples": []}
         elif level not in new_structure[cluster_num] and level > 1:
-            new_structure[cluster_num][level] = {
-                "samples": deepcopy(new_structure[cluster_num][level - 1]["samples"])
-            }
+            new_structure[cluster_num][level] = {"samples": deepcopy(new_structure[cluster_num][level - 1]["samples"])}
 
         # Extending the samples list.
         new_structure[cluster_num][level]["samples"].extend(samples)
 
     return new_structure
 
 
@@ -158,17 +149,15 @@
 
     for _, values in clusters.items():
         if values["samples_added"]:
             level = values["level"]
             cluster = values["cluster_num"]
             for sample in values["samples_added"]:
                 sample_tracking[sample]["cluster"][level] = values["cluster_num"]
-                sample_tracking[sample]["distance"][level, cluster] = values[
-                    "sample_dist"
-                ]
+                sample_tracking[sample]["distance"][level, cluster] = values["sample_dist"]
                 sample_tracking[sample]["distance"][level, :] = get_distance(
                     cluster,
                     level,
                     sample,
                     sample_tracking[sample]["distance"][level, :],
                     distance_matrix,
                     sample_clusters,
```

### Comparing `daml-0.51.0/src/daml/metrics/__init__.py` & `daml-0.52.0/src/daml/metrics/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,21 +3,18 @@
 from daml._internal.metrics.ber import BER
 from daml._internal.metrics.divergence import Divergence
 from daml._internal.metrics.uap import UAP
 from daml.metrics import drift
 
 __all__ = ["BER", "Divergence", "UAP", "drift"]
 
-if (
-    find_spec("tensorflow") is not None
-    and find_spec("tensorflow_probability") is not None
-):  # pragma: no cover
-    from . import outlier_detection
+if find_spec("tensorflow") is not None and find_spec("tensorflow_probability") is not None:  # pragma: no cover
+    from . import outlier
 
-    __all__ += ["outlier_detection"]
+    __all__ += ["outlier"]
 
 if find_spec("torch") is not None:  # pragma: no cover
     from daml._internal.metrics.sufficiency import Sufficiency
 
     __all__ += ["Sufficiency"]
 
 del find_spec
```

### Comparing `daml-0.51.0/src/daml/metrics/drift/__init__.py` & `daml-0.52.0/src/daml/metrics/drift/__init__.py`

 * *Files identical despite different names*

### Comparing `daml-0.51.0/PKG-INFO` & `daml-0.52.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: daml
-Version: 0.51.0
+Version: 0.52.0
 Summary: DAML provides a simple interface to characterize image data and its impact on model performance across classification and object-detection tasks
 Home-page: https://daml.ai/
 License: MIT
 Author: Andrew Weng
 Author-email: andrew.weng@ariacoustics.com
 Maintainer: ARiA
 Maintainer-email: daml@ariacoustics.com
```

