# Comparing `tmp/tensorkrowch-1.1.1.tar.gz` & `tmp/tensorkrowch-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tensorkrowch-1.1.1.tar", last modified: Thu Apr 18 22:43:14 2024, max compression
+gzip compressed data, was "tensorkrowch-1.1.2.tar", last modified: Fri May 10 08:17:47 2024, max compression
```

## Comparing `tensorkrowch-1.1.1.tar` & `tensorkrowch-1.1.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxr-x   0 jose      (1000) jose      (1000)        0 2024-04-18 22:43:14.802905 tensorkrowch-1.1.1/
--rw-rw-r--   0 jose      (1000) jose      (1000)     1086 2023-05-25 11:43:07.000000 tensorkrowch-1.1.1/LICENSE.txt
--rw-rw-r--   0 jose      (1000) jose      (1000)       11 2024-03-06 17:59:45.000000 tensorkrowch-1.1.1/MANIFEST.in
--rw-r--r--   0 jose      (1000) jose      (1000)     8770 2024-04-18 22:43:14.802905 tensorkrowch-1.1.1/PKG-INFO
--rw-rw-r--   0 jose      (1000) jose      (1000)     6358 2024-04-14 00:27:40.000000 tensorkrowch-1.1.1/README.md
--rw-rw-r--   0 jose      (1000) jose      (1000)     1349 2024-04-14 00:06:08.000000 tensorkrowch-1.1.1/pyproject.toml
--rw-rw-r--   0 jose      (1000) jose      (1000)       38 2024-04-18 22:43:14.802905 tensorkrowch-1.1.1/setup.cfg
--rw-rw-r--   0 jose      (1000) jose      (1000)       38 2024-03-06 17:59:45.000000 tensorkrowch-1.1.1/setup.py
-drwxrwxr-x   0 jose      (1000) jose      (1000)        0 2024-04-18 22:43:14.798905 tensorkrowch-1.1.1/tensorkrowch/
--rw-rw-r--   0 jose      (1000) jose      (1000)     1382 2024-04-18 22:42:39.000000 tensorkrowch-1.1.1/tensorkrowch/__init__.py
--rw-rw-r--   0 jose      (1000) jose      (1000)   198461 2024-04-17 22:16:33.000000 tensorkrowch-1.1.1/tensorkrowch/components.py
-drwxrwxr-x   0 jose      (1000) jose      (1000)        0 2024-04-18 22:43:14.798905 tensorkrowch-1.1.1/tensorkrowch/decompositions/
--rw-rw-r--   0 jose      (1000) jose      (1000)       81 2024-04-14 00:28:38.000000 tensorkrowch-1.1.1/tensorkrowch/decompositions/__init__.py
--rw-rw-r--   0 jose      (1000) jose      (1000)    10787 2024-04-14 08:34:34.000000 tensorkrowch-1.1.1/tensorkrowch/decompositions/svd_decompositions.py
--rw-rw-r--   0 jose      (1000) jose      (1000)    13298 2024-04-17 18:24:11.000000 tensorkrowch-1.1.1/tensorkrowch/embeddings.py
--rw-rw-r--   0 jose      (1000) jose      (1000)     6401 2024-04-18 08:40:07.000000 tensorkrowch-1.1.1/tensorkrowch/initializers.py
-drwxrwxr-x   0 jose      (1000) jose      (1000)        0 2024-04-18 22:43:14.798905 tensorkrowch-1.1.1/tensorkrowch/models/
--rw-rw-r--   0 jose      (1000) jose      (1000)      384 2024-04-14 00:06:08.000000 tensorkrowch-1.1.1/tensorkrowch/models/__init__.py
--rw-rw-r--   0 jose      (1000) jose      (1000)    50650 2024-04-18 20:01:59.000000 tensorkrowch-1.1.1/tensorkrowch/models/mpo.py
--rw-rw-r--   0 jose      (1000) jose      (1000)   174436 2024-04-18 22:39:56.000000 tensorkrowch-1.1.1/tensorkrowch/models/mps.py
--rw-rw-r--   0 jose      (1000) jose      (1000)    21760 2024-04-14 08:41:17.000000 tensorkrowch-1.1.1/tensorkrowch/models/mps_data.py
--rw-rw-r--   0 jose      (1000) jose      (1000)    58352 2024-04-18 22:38:24.000000 tensorkrowch-1.1.1/tensorkrowch/models/peps.py
--rw-rw-r--   0 jose      (1000) jose      (1000)    37360 2024-03-06 17:59:45.000000 tensorkrowch-1.1.1/tensorkrowch/models/tree.py
--rw-rw-r--   0 jose      (1000) jose      (1000)   181888 2024-04-18 22:37:53.000000 tensorkrowch-1.1.1/tensorkrowch/operations.py
--rw-rw-r--   0 jose      (1000) jose      (1000)     9156 2024-04-14 00:06:08.000000 tensorkrowch-1.1.1/tensorkrowch/utils.py
-drwxrwxr-x   0 jose      (1000) jose      (1000)        0 2024-04-18 22:43:14.798905 tensorkrowch-1.1.1/tensorkrowch.egg-info/
--rw-r--r--   0 jose      (1000) jose      (1000)     8770 2024-04-18 22:43:14.000000 tensorkrowch-1.1.1/tensorkrowch.egg-info/PKG-INFO
--rw-rw-r--   0 jose      (1000) jose      (1000)      657 2024-04-18 22:43:14.000000 tensorkrowch-1.1.1/tensorkrowch.egg-info/SOURCES.txt
--rw-rw-r--   0 jose      (1000) jose      (1000)        1 2024-04-18 22:43:14.000000 tensorkrowch-1.1.1/tensorkrowch.egg-info/dependency_links.txt
--rw-rw-r--   0 jose      (1000) jose      (1000)      270 2024-04-18 22:43:14.000000 tensorkrowch-1.1.1/tensorkrowch.egg-info/requires.txt
--rw-rw-r--   0 jose      (1000) jose      (1000)       13 2024-04-18 22:43:14.000000 tensorkrowch-1.1.1/tensorkrowch.egg-info/top_level.txt
+drwxrwxr-x   0 jose      (1000) jose      (1000)        0 2024-05-10 08:17:47.743049 tensorkrowch-1.1.2/
+-rw-rw-r--   0 jose      (1000) jose      (1000)     1086 2023-05-25 11:43:07.000000 tensorkrowch-1.1.2/LICENSE.txt
+-rw-rw-r--   0 jose      (1000) jose      (1000)       11 2024-03-06 17:59:45.000000 tensorkrowch-1.1.2/MANIFEST.in
+-rw-r--r--   0 jose      (1000) jose      (1000)    10354 2024-05-10 08:17:47.743049 tensorkrowch-1.1.2/PKG-INFO
+-rw-rw-r--   0 jose      (1000) jose      (1000)     7808 2024-05-10 08:16:58.000000 tensorkrowch-1.1.2/README.md
+-rw-rw-r--   0 jose      (1000) jose      (1000)     1482 2024-05-10 08:16:58.000000 tensorkrowch-1.1.2/pyproject.toml
+-rw-rw-r--   0 jose      (1000) jose      (1000)       38 2024-05-10 08:17:47.743049 tensorkrowch-1.1.2/setup.cfg
+-rw-rw-r--   0 jose      (1000) jose      (1000)       38 2024-03-06 17:59:45.000000 tensorkrowch-1.1.2/setup.py
+drwxrwxr-x   0 jose      (1000) jose      (1000)        0 2024-05-10 08:17:47.739049 tensorkrowch-1.1.2/tensorkrowch/
+-rw-rw-r--   0 jose      (1000) jose      (1000)     1382 2024-05-10 08:16:58.000000 tensorkrowch-1.1.2/tensorkrowch/__init__.py
+-rw-rw-r--   0 jose      (1000) jose      (1000)   198461 2024-05-09 19:05:34.000000 tensorkrowch-1.1.2/tensorkrowch/components.py
+drwxrwxr-x   0 jose      (1000) jose      (1000)        0 2024-05-10 08:17:47.739049 tensorkrowch-1.1.2/tensorkrowch/decompositions/
+-rw-rw-r--   0 jose      (1000) jose      (1000)       81 2024-05-10 08:17:27.000000 tensorkrowch-1.1.2/tensorkrowch/decompositions/__init__.py
+-rw-rw-r--   0 jose      (1000) jose      (1000)    10787 2024-05-09 20:25:43.000000 tensorkrowch-1.1.2/tensorkrowch/decompositions/svd_decompositions.py
+-rw-rw-r--   0 jose      (1000) jose      (1000)    13298 2024-04-18 22:46:59.000000 tensorkrowch-1.1.2/tensorkrowch/embeddings.py
+-rw-rw-r--   0 jose      (1000) jose      (1000)     6401 2024-04-18 22:46:59.000000 tensorkrowch-1.1.2/tensorkrowch/initializers.py
+drwxrwxr-x   0 jose      (1000) jose      (1000)        0 2024-05-10 08:17:47.743049 tensorkrowch-1.1.2/tensorkrowch/models/
+-rw-rw-r--   0 jose      (1000) jose      (1000)      384 2024-04-14 00:06:08.000000 tensorkrowch-1.1.2/tensorkrowch/models/__init__.py
+-rw-rw-r--   0 jose      (1000) jose      (1000)    51467 2024-05-10 08:16:58.000000 tensorkrowch-1.1.2/tensorkrowch/models/mpo.py
+-rw-rw-r--   0 jose      (1000) jose      (1000)   179253 2024-05-10 08:16:58.000000 tensorkrowch-1.1.2/tensorkrowch/models/mps.py
+-rw-rw-r--   0 jose      (1000) jose      (1000)    21760 2024-04-18 22:46:59.000000 tensorkrowch-1.1.2/tensorkrowch/models/mps_data.py
+-rw-rw-r--   0 jose      (1000) jose      (1000)    58352 2024-04-18 22:46:59.000000 tensorkrowch-1.1.2/tensorkrowch/models/peps.py
+-rw-rw-r--   0 jose      (1000) jose      (1000)    37360 2024-03-06 17:59:45.000000 tensorkrowch-1.1.2/tensorkrowch/models/tree.py
+-rw-rw-r--   0 jose      (1000) jose      (1000)   182494 2024-05-10 08:16:58.000000 tensorkrowch-1.1.2/tensorkrowch/operations.py
+-rw-rw-r--   0 jose      (1000) jose      (1000)     9156 2024-04-14 00:06:08.000000 tensorkrowch-1.1.2/tensorkrowch/utils.py
+drwxrwxr-x   0 jose      (1000) jose      (1000)        0 2024-05-10 08:17:47.743049 tensorkrowch-1.1.2/tensorkrowch.egg-info/
+-rw-r--r--   0 jose      (1000) jose      (1000)    10354 2024-05-10 08:17:47.000000 tensorkrowch-1.1.2/tensorkrowch.egg-info/PKG-INFO
+-rw-rw-r--   0 jose      (1000) jose      (1000)      657 2024-05-10 08:17:47.000000 tensorkrowch-1.1.2/tensorkrowch.egg-info/SOURCES.txt
+-rw-rw-r--   0 jose      (1000) jose      (1000)        1 2024-05-10 08:17:47.000000 tensorkrowch-1.1.2/tensorkrowch.egg-info/dependency_links.txt
+-rw-rw-r--   0 jose      (1000) jose      (1000)      307 2024-05-10 08:17:47.000000 tensorkrowch-1.1.2/tensorkrowch.egg-info/requires.txt
+-rw-rw-r--   0 jose      (1000) jose      (1000)       13 2024-05-10 08:17:47.000000 tensorkrowch-1.1.2/tensorkrowch.egg-info/top_level.txt
```

### Comparing `tensorkrowch-1.1.1/LICENSE.txt` & `tensorkrowch-1.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tensorkrowch-1.1.1/PKG-INFO` & `tensorkrowch-1.1.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tensorkrowch
-Version: 1.1.1
+Version: 1.1.2
 Summary: Tensor Networks with PyTorch
 Author-email: José Ramón Pareja Monturiol <joserapa98@gmail.com>
 Maintainer-email: José Ramón Pareja Monturiol <joserapa98@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 José Ramón Pareja Monturiol
         
@@ -32,23 +32,26 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: torch>=1.9
 Requires-Dist: opt_einsum>=3.0
 Provides-Extra: tests
 Requires-Dist: pytest; extra == "tests"
+Requires-Dist: pytest-cov; extra == "tests"
 Provides-Extra: docs
 Requires-Dist: sphinx==4.5.0; extra == "docs"
 Requires-Dist: sphinx-book-theme==0.3.3; extra == "docs"
 Requires-Dist: sphinx-copybutton==0.5.2; extra == "docs"
 Requires-Dist: sphinxcontrib-applehelp==1.0.4; extra == "docs"
 Requires-Dist: sphinxcontrib-devhelp==1.0.2; extra == "docs"
 Requires-Dist: sphinxcontrib-htmlhelp==2.0.1; extra == "docs"
 Requires-Dist: sphinxcontrib-qthelp==1.0.3; extra == "docs"
 Requires-Dist: sphinxcontrib-serializinghtml==1.1.5; extra == "docs"
+Requires-Dist: ipykernel; extra == "docs"
+Requires-Dist: nbsphinx==0.9.3; extra == "docs"
 
 ![logo](https://github.com/joserapa98/tensorkrowch/blob/master/docs/figures/svg/tensorkrowch_logo_dark.svg#gh-dark-mode-only)
 ![logo](https://github.com/joserapa98/tensorkrowch/blob/master/docs/figures/svg/tensorkrowch_logo_light.svg#gh-light-mode-only)
 
 [![DOI](https://zenodo.org/badge/453954432.svg)](https://zenodo.org/badge/latestdoi/453954432)
 
 # Tensor Networks with PyTorch
@@ -123,14 +126,20 @@
 
 ```
 python -m pytest -v
 ```
 
 inside the repository folder.
 
+> [!NOTE]
+Certain tests may experience failure as a result of statistical anomalies or 
+hardware constraints. We advise reviewing the error messages to determine if 
+these failures stem from such occurrences. Should this be the case, consider 
+rerunning the tests to ascertain if the errors persist.
+
 
 ## Example
 
 With **TensorKrowch** you can experiment building Tensor Networks:
 
 ```python
 import torch
@@ -200,14 +209,33 @@
 * [Contracting and Differentiating the Tensor Network](https://joserapa98.github.io/tensorkrowch/_build/html/tutorials/2_contracting_tensor_network.html)
 * [How to save Memory and Time with TensorKrowch (ADVANCED)](https://joserapa98.github.io/tensorkrowch/_build/html/tutorials/3_memory_management.html)
 * [The different Types of Nodes (ADVANCED)](https://joserapa98.github.io/tensorkrowch/_build/html/tutorials/4_types_of_nodes.html)
 * [How to subclass TensorNetwork to build Custom Models](https://joserapa98.github.io/tensorkrowch/_build/html/tutorials/5_subclass_tensor_network.html)
 * [Creating a Hybrid Neural-Tensor Network Model](https://joserapa98.github.io/tensorkrowch/_build/html/tutorials/6_mix_with_pytorch.html)
 
 
+## Example Notebooks
+
+In addition to the informative tutorials, there is also a collection of examples
+that serve as practical demonstrations of how to apply **TensorKrowch** in
+various contexts, showcasing its versatility.
+
+With the code provided in the examples, you will be able to reproduce key research
+findings that bridge the gap between tensor networks and machine learning. These
+examples provide a hands-on approach to understanding the intricacies of
+**TensorKrowch**, allowing you to explore its potential and adapt it to your
+specific needs.
+
+* [Training MPS in different ways](https://joserapa98.github.io/tensorkrowch/_build/html/examples/training_mps.html)
+* [Hybrid Tensorial Neural Network model](https://joserapa98.github.io/tensorkrowch/_build/html/examples/hybrid_tnn_model.html)
+* [Tensorizing Neural Networks](https://joserapa98.github.io/tensorkrowch/_build/html/examples/tensorizing_nn.html)
+* [DMRG-like training of MPS](https://joserapa98.github.io/tensorkrowch/_build/html/examples/mps_dmrg.html)
+* [Hybrid DMRG-like training of MPS](https://joserapa98.github.io/tensorkrowch/_build/html/examples/mps_dmrg_hybrid.html)
+
+
 ## License
 
 TensorKrowch is licensed under the MIT License. Please see the [LICENSE](https://github.com/joserapa98/tensorkrowch/blob/master/LICENSE.txt) file for more information.
 
 
 ## Citing
```

### Comparing `tensorkrowch-1.1.1/README.md` & `tensorkrowch-1.1.2/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -75,14 +75,20 @@
 
 ```
 python -m pytest -v
 ```
 
 inside the repository folder.
 
+> [!NOTE]
+Certain tests may experience failure as a result of statistical anomalies or 
+hardware constraints. We advise reviewing the error messages to determine if 
+these failures stem from such occurrences. Should this be the case, consider 
+rerunning the tests to ascertain if the errors persist.
+
 
 ## Example
 
 With **TensorKrowch** you can experiment building Tensor Networks:
 
 ```python
 import torch
@@ -152,14 +158,33 @@
 * [Contracting and Differentiating the Tensor Network](https://joserapa98.github.io/tensorkrowch/_build/html/tutorials/2_contracting_tensor_network.html)
 * [How to save Memory and Time with TensorKrowch (ADVANCED)](https://joserapa98.github.io/tensorkrowch/_build/html/tutorials/3_memory_management.html)
 * [The different Types of Nodes (ADVANCED)](https://joserapa98.github.io/tensorkrowch/_build/html/tutorials/4_types_of_nodes.html)
 * [How to subclass TensorNetwork to build Custom Models](https://joserapa98.github.io/tensorkrowch/_build/html/tutorials/5_subclass_tensor_network.html)
 * [Creating a Hybrid Neural-Tensor Network Model](https://joserapa98.github.io/tensorkrowch/_build/html/tutorials/6_mix_with_pytorch.html)
 
 
+## Example Notebooks
+
+In addition to the informative tutorials, there is also a collection of examples
+that serve as practical demonstrations of how to apply **TensorKrowch** in
+various contexts, showcasing its versatility.
+
+With the code provided in the examples, you will be able to reproduce key research
+findings that bridge the gap between tensor networks and machine learning. These
+examples provide a hands-on approach to understanding the intricacies of
+**TensorKrowch**, allowing you to explore its potential and adapt it to your
+specific needs.
+
+* [Training MPS in different ways](https://joserapa98.github.io/tensorkrowch/_build/html/examples/training_mps.html)
+* [Hybrid Tensorial Neural Network model](https://joserapa98.github.io/tensorkrowch/_build/html/examples/hybrid_tnn_model.html)
+* [Tensorizing Neural Networks](https://joserapa98.github.io/tensorkrowch/_build/html/examples/tensorizing_nn.html)
+* [DMRG-like training of MPS](https://joserapa98.github.io/tensorkrowch/_build/html/examples/mps_dmrg.html)
+* [Hybrid DMRG-like training of MPS](https://joserapa98.github.io/tensorkrowch/_build/html/examples/mps_dmrg_hybrid.html)
+
+
 ## License
 
 TensorKrowch is licensed under the MIT License. Please see the [LICENSE](https://github.com/joserapa98/tensorkrowch/blob/master/LICENSE.txt) file for more information.
 
 
 ## Citing
```

### Comparing `tensorkrowch-1.1.1/pyproject.toml` & `tensorkrowch-1.1.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -27,26 +27,30 @@
 dependencies = [
   "torch>=1.9",
   "opt_einsum>=3.0",
 ]
 
 
 [project.optional-dependencies]
-tests = ["pytest"]
+tests = ["pytest", "pytest-cov"]
 docs = [
     "sphinx==4.5.0",
     "sphinx-book-theme==0.3.3",
     "sphinx-copybutton==0.5.2",
     "sphinxcontrib-applehelp==1.0.4",
     "sphinxcontrib-devhelp==1.0.2",
     "sphinxcontrib-htmlhelp==2.0.1",
     "sphinxcontrib-qthelp==1.0.3",
-    "sphinxcontrib-serializinghtml==1.1.5"
+    "sphinxcontrib-serializinghtml==1.1.5",
+    "ipykernel",
+    "nbsphinx==0.9.3"
 ]
 
+# To run nbsphinx, pandoc should be installed via conda: conda install pandoc
+
 
 [tool.setuptools.dynamic]
 version = {attr = "tensorkrowch.__version__"}
 readme = {file = "README.md", content-type = "text/markdown"}
 
 
 [tool.setuptools]
```

### Comparing `tensorkrowch-1.1.1/tensorkrowch/__init__.py` & `tensorkrowch-1.1.2/tensorkrowch/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 TensorKrowch
 ============
 
 Tensor Networks with PyTorch
 """
 
 # Version
-__version__ = '1.1.1'
+__version__ = '1.1.2'
 
 # Network components
 from tensorkrowch.components import Axis
 from tensorkrowch.components import AbstractNode, Node, ParamNode
 from tensorkrowch.components import StackNode, ParamStackNode
 from tensorkrowch.components import Edge, StackEdge
 from tensorkrowch.components import Successor, TensorNetwork
```

### Comparing `tensorkrowch-1.1.1/tensorkrowch/components.py` & `tensorkrowch-1.1.2/tensorkrowch/components.py`

 * *Files identical despite different names*

### Comparing `tensorkrowch-1.1.1/tensorkrowch/decompositions/svd_decompositions.py` & `tensorkrowch-1.1.2/tensorkrowch/decompositions/svd_decompositions.py`

 * *Files identical despite different names*

### Comparing `tensorkrowch-1.1.1/tensorkrowch/embeddings.py` & `tensorkrowch-1.1.2/tensorkrowch/embeddings.py`

 * *Files identical despite different names*

### Comparing `tensorkrowch-1.1.1/tensorkrowch/initializers.py` & `tensorkrowch-1.1.2/tensorkrowch/initializers.py`

 * *Files identical despite different names*

### Comparing `tensorkrowch-1.1.1/tensorkrowch/models/mpo.py` & `tensorkrowch-1.1.2/tensorkrowch/models/mpo.py`

 * *Files 1% similar despite different names*

```diff
@@ -328,14 +328,23 @@
         return self._right_node
     
     @property
     def mats_env(self) -> List[AbstractNode]:
         """Returns the list of nodes in ``mats_env``."""
         return self._mats_env
     
+    @property
+    def tensors(self) -> List[torch.Tensor]:
+        """Returns the list of MPO tensors."""
+        mpo_tensors = [node.tensor for node in self._mats_env]
+        if self._boundary == 'obc':
+            mpo_tensors[0] = mpo_tensors[0][0, :, :]
+            mpo_tensors[-1] = mpo_tensors[-1][:, :, 0]
+        return mpo_tensors
+    
     # -------
     # Methods
     # -------
     def _make_nodes(self) -> None:
         """Creates all the nodes of the MPO."""
         if self._leaf_nodes:
             raise ValueError('Cannot create MPO nodes if the MPO already has '
@@ -544,14 +553,24 @@
         
         if net._boundary == 'obc':
             net._left_node = net._left_node.parameterize(set_param)
             net._right_node = net._right_node.parameterize(set_param)
             
         return net
     
+    def update_bond_dim(self) -> None:
+        """
+        Updates the :attr:`bond_dim` attribute of the ``MPO``, in case it is
+        outdated.
+        """
+        if self._boundary == 'obc':
+            self._bond_dim = [node.shape[2] for node in self._mats_env[:-1]]
+        else:
+            self._bond_dim = [node.shape[2] for node in self._mats_env]
+    
     def _input_contraction(self,
                            nodes_env: List[AbstractNode],
                            input_nodes: List[AbstractNode],
                            inline_input: bool = False) -> Tuple[
                                                        Optional[List[Node]],
                                                        Optional[List[Node]]]:
         """Contracts input data nodes with MPO nodes."""
@@ -625,24 +644,24 @@
 
             stack1 = op.stack(even_nodes)
             stack2 = op.stack(odd_nodes)
 
             stack1 ^ stack2
 
             aux_nodes = stack1 @ stack2
-            aux_nodes = op.unbind(aux_nodes)
             
             if renormalize:
-                for i in range(len(aux_nodes)):
-                    axes = []
-                    for ax_name in aux_nodes[i].axes_names:
-                        if ('left' in ax_name) or ('right' in ax_name):
-                            axes.append(ax_name)
-                    if axes:
-                        aux_nodes[i] = aux_nodes[i].renormalize(axis=axes)
+                axes = []
+                for ax_name in aux_nodes.axes_names:
+                    if ('left' in ax_name) or ('right' in ax_name):
+                        axes.append(ax_name)
+                if axes:
+                    aux_nodes = aux_nodes.renormalize(axis=axes)
+            
+            aux_nodes = op.unbind(aux_nodes)
 
             return aux_nodes, leftover
         return mats_env, []
 
     def _pairwise_contraction(self,
                               mats_env: List[Node],
                               mps: Optional[MPSData] = None,
@@ -796,14 +815,19 @@
         equally for all SVD computations.
         
         If none of them are specified, the bond dimensions won't be modified
         if possible. Only when the bond dimension is bigger than the physical
         dimension multiplied by the other bond dimension of the node, it will
         be cropped to that size.
         
+        If rank is not specified, the current bond dimensions will be used as
+        the rank. That is, the current bond dimensions will be the upper bound
+        for the possibly new bond dimensions given by the arguments
+        ``cum_percentage`` and/or ``cutoff``.
+        
         Parameters
         ----------
         oc : int
             Position of the orthogonality center. It should be between 0 and 
             ``n_features - 1``.
         mode : {"svd", "svdr", "qr"}
             Indicates which decomposition should be used to split a node after
@@ -862,15 +886,15 @@
                 nodes[0].tensor[1:])
             nodes[-1].tensor[..., 1:, :] = torch.zeros_like(
                 nodes[-1].tensor[..., 1:, :])
         
         # If mode is svd or svr and none of the args is provided, the ranks are
         # kept as they were originally
         keep_rank = False
-        if (rank is None) and (cum_percentage is None) and (cutoff is None):
+        if rank is None:
             keep_rank = True
         
         for i in range(oc):
             if mode == 'svd':
                 result1, result2 = nodes[i]['right'].svd_(
                     side='right',
                     rank=nodes[i]['right'].size() if keep_rank else rank,
@@ -884,15 +908,15 @@
                     cutoff=cutoff)
             elif mode == 'qr':
                 result1, result2 = nodes[i]['right'].qr_()
             else:
                 raise ValueError('`mode` can only be "svd", "svdr" or "qr"')
             
             if renormalize:
-                aux_norm = result2.norm() / sqrt(result2.shape[0])
+                aux_norm = result2.norm()
                 if not aux_norm.isinf() and (aux_norm > 0):
                     result2.tensor = result2.tensor / aux_norm
                     log_norm += aux_norm.log()
 
             result1 = result1.parameterize()
             nodes[i] = result1
             nodes[i + 1] = result2
@@ -912,15 +936,15 @@
                     cutoff=cutoff)
             elif mode == 'qr':
                 result1, result2 = nodes[i]['left'].rq_()
             else:
                 raise ValueError('`mode` can only be "svd", "svdr" or "qr"')
             
             if renormalize:
-                aux_norm = result1.norm() / sqrt(result1.shape[0])
+                aux_norm = result1.norm()
                 if not aux_norm.isinf() and (aux_norm > 0):
                     result1.tensor = result1.tensor / aux_norm
                     log_norm += aux_norm.log()
 
             result2 = result2.parameterize()
             nodes[i] = result2
             nodes[i - 1] = result1
```

### Comparing `tensorkrowch-1.1.1/tensorkrowch/models/mps.py` & `tensorkrowch-1.1.2/tensorkrowch/models/mps.py`

 * *Files 0% similar despite different names*

```diff
@@ -512,14 +512,23 @@
         """Returns the list of input nodes."""
         return [self._mats_env[i] for i in self._in_features]
     
     @property
     def out_env(self) -> List[AbstractNode]:
         """Returns the list of output nodes."""
         return [self._mats_env[i] for i in self._out_features]
+
+    @property
+    def tensors(self) -> List[torch.Tensor]:
+        """Returns the list of MPS tensors."""
+        mps_tensors = [node.tensor for node in self._mats_env]
+        if self._boundary == 'obc':
+            mps_tensors[0] = mps_tensors[0][0, :, :]
+            mps_tensors[-1] = mps_tensors[-1][:, :, 0]
+        return mps_tensors
     
     # -------
     # Methods
     # -------
     def _make_nodes(self) -> None:
         """Creates all the nodes of the MPS."""
         if self._leaf_nodes:
@@ -839,14 +848,24 @@
             net._mats_env[i] = net._mats_env[i].parameterize(set_param)
         
         if net._boundary == 'obc':
             net._left_node = net._left_node.parameterize(set_param)
             net._right_node = net._right_node.parameterize(set_param)
             
         return net
+    
+    def update_bond_dim(self) -> None:
+        """
+        Updates the :attr:`bond_dim` attribute of the ``MPS``, in case it is
+        outdated.
+        """
+        if self._boundary == 'obc':
+            self._bond_dim = [node.shape[-1] for node in self._mats_env[:-1]]
+        else:
+            self._bond_dim = [node.shape[-1] for node in self._mats_env]
 
     def _input_contraction(self,
                            nodes_env: List[AbstractNode],
                            input_nodes: List[AbstractNode],
                            inline_input: bool = False) -> Tuple[
                                                        Optional[List[Node]],
                                                        Optional[List[Node]]]:
@@ -938,24 +957,24 @@
 
             stack1 = op.stack(even_nodes)
             stack2 = op.stack(odd_nodes)
 
             stack1['right'] ^ stack2['left']
 
             aux_nodes = stack1 @ stack2
-            aux_nodes = op.unbind(aux_nodes)
             
             if renormalize:
-                for i in range(len(aux_nodes)):
-                    axes = []
-                    for ax_name in aux_nodes[i].axes_names:
-                        if ('left' in ax_name) or ('right' in ax_name):
-                            axes.append(ax_name)
-                    if axes:
-                        aux_nodes[i] = aux_nodes[i].renormalize(axis=axes)
+                axes = []
+                for ax_name in aux_nodes.axes_names:
+                    if ('left' in ax_name) or ('right' in ax_name):
+                        axes.append(ax_name)
+                if axes:
+                    aux_nodes = aux_nodes.renormalize(axis=axes)
+            
+            aux_nodes = op.unbind(aux_nodes)
 
             return aux_nodes, leftover
         return mats_env, []
 
     def _pairwise_contraction(self,
                               mats_env: List[AbstractNode],
                               renormalize: bool = False) -> Node:
@@ -1165,15 +1184,15 @@
                         aux_out_env[0] = self._left_node @ aux_out_env[0]
                 else:
                     aux_out_env[0] = in_results[i - out_first] @ aux_out_env[0]
                 
                 nodes_out_env += aux_out_env
             
             if out_last:
-                if (self._boundary == 'obc'):
+                if self._boundary == 'obc':
                     nodes_out_env[-1] = nodes_out_env[-1] @ self._right_node
             else:
                 nodes_out_env[-1] = nodes_out_env[-1] @ in_results[-1]
             
             if not marginalize_output:
                 # Contract all output nodes sequentially
                 result = self._inline_contraction(mats_env=nodes_out_env,
@@ -1300,32 +1319,131 @@
         
         all_edges = batch_edges + other_edges
         if all_edges != list(range(len(all_edges))):
             result = op.permute(result, tuple(all_edges))
         
         return result
     
-    def norm(self) -> torch.Tensor:
+    def norm(self,
+             log_scale: bool = False) -> torch.Tensor:
         """
         Computes the norm of the MPS.
         
-        This method internally sets ``in_features = []``, and calls the
-        :meth:`~tensorkrowch.TensorNetwork.forward` method with
-        ``marginalize_output = True``. Therefore, it may alter the behaviour
-        of the MPS if it is not :meth:`~tensorkrowch.TensorNetwork.reset`
-        afterwards. Also, if the MPS was contracted before with other arguments,
-        it should be ``reset`` before calling ``norm`` to avoid undesired
-        behaviour.
+        This method internally removes all data nodes in the MPS, if any, and
+        contracts the nodes with themselves. Therefore, this may alter the
+        usual behaviour of :meth:`contract` if the MPS is not
+        :meth:`~tensorkrowch.TensorNetwork.reset` afterwards. Also, if the MPS
+        was contracted before with other arguments, it should be ``reset``
+        before calling ``norm`` to avoid undesired behaviour.
+        
+        Since the norm is computed by contracting the MPS, it means one can
+        take gradients of it with respect to the MPS tensors, if it is needed.
+        
+        Parameters
+        ----------
+        log_scale : bool
+            Boolean indicating whether the resulting norm should be given in
+            logarithmoc scale. Useful for cases where the norm explodes or
+            vanishes.
         """
         if self._data_nodes:
             self.unset_data_nodes()
-        self.in_features = []
         
-        result = self.forward(marginalize_output=True)
-        result = result.sqrt()
+        # All nodes belong to the output region
+        all_nodes = self.mats_env[:]
+        
+        if self._boundary == 'obc':
+            all_nodes[0] = self._left_node @ all_nodes[0]
+            all_nodes[-1] = all_nodes[-1] @ self._right_node
+        
+        # Check if nodes are already connected to copied nodes
+        create_copies = []
+        for node in all_nodes:
+            neighbour = node.neighbours('input')
+            if neighbour is None:
+                create_copies.append(True)
+            else:
+                if 'virtual_result_copy' not in neighbour.name:
+                    raise ValueError(
+                        f'Node {node} is already connected to another node '
+                        'at axis "input". Disconnect the node or reset the '
+                        'network before calling `norm`')
+                else:
+                    create_copies.append(False)
+        
+        if any(create_copies) and not all(create_copies):
+            raise ValueError(
+                'There are some nodes connected and some disconnected at axis '
+                '"input". Disconnect all of them before calling `norm`')
+        
+        create_copies = any(create_copies)
+        
+        # Copy output nodes sharing tensors
+        if create_copies:
+            copied_nodes = []
+            for node in all_nodes:
+                copied_node = node.__class__(shape=node._shape,
+                                             axes_names=node.axes_names,
+                                             name='virtual_result_copy',
+                                             network=self,
+                                             virtual=True)
+                copied_node.set_tensor_from(node)
+                copied_nodes.append(copied_node)
+                
+                # Change batch names so that they not coincide with
+                # original batches, which gives dupliicate output batches
+                for ax in copied_node.axes:
+                    if ax._batch:
+                        ax.name = ax.name + '_copy'
+            
+            # Connect copied nodes with neighbours
+            for i in range(len(copied_nodes)):
+                if (i == 0) and (self._boundary == 'pbc'):
+                    if all_nodes[i - 1].is_connected_to(all_nodes[i]):
+                        copied_nodes[i - 1]['right'] ^ copied_nodes[i]['left']
+                elif i > 0:
+                    copied_nodes[i - 1]['right'] ^ copied_nodes[i]['left']
+            
+            # Reattach input edges of resultant output nodes and connect
+            # with copied nodes
+            for node, copied_node in zip(all_nodes, copied_nodes):
+                # Reattach input edges
+                node.reattach_edges(axes=['input'])
+                
+                # Connect copies directly to output nodes
+                copied_node['input'] ^ node['input']
+        else:
+            copied_nodes = []
+            for node in all_nodes:
+                copied_nodes.append(node.neighbours('input'))
+            
+        # Contract output nodes with copies
+        mats_out_env = self._input_contraction(
+            nodes_env=all_nodes,
+            input_nodes=copied_nodes,
+            inline_input=True)
+        
+        # Contract resultant matrices
+        log_norm = 0
+        result_node = mats_out_env[0]
+        if log_scale:
+            log_norm += result_node.norm()
+            result_node = result_node.renormalize()
+                
+        for node in mats_out_env[1:]:
+            result_node @= node
+            
+            if log_scale:
+                log_norm += result_node.norm()
+                result_node = result_node.renormalize()
+        
+        if log_scale:
+            return log_norm / 2
+        
+        result = result_node.tensor.sqrt()
         return result
 
     def partial_density(self,
                         trace_sites: Sequence[int] = [],
                         renormalize: bool = True) -> torch.Tensor:
         r"""
         Returns de partial density matrix, tracing out the sites specified
@@ -1380,17 +1498,18 @@
                 raise TypeError(
                     'elements of `trace_sites` should be int type')
             if (site < 0) or (site >= self._n_features):
                 raise ValueError(
                     'Elements of `trace_sites` should be between 0 and '
                     '(`n_features` - 1)')
         
-        if self._data_nodes:
-            self.unset_data_nodes()
-        self.out_features = trace_sites
+        if set(trace_sites) != set(self.out_features):
+            if self._data_nodes:
+                self.unset_data_nodes()
+            self.out_features = trace_sites
         
         # Create dataset with all possible combinations for the input nodes
         # so that they are kept sort of "open"
         dims = torch.tensor([self._phys_dim[i] for i in self._in_features])
         
         data = []
         for i in range(len(self._in_features)):
@@ -1416,14 +1535,18 @@
                                   renormalize=renormalize,
                                   marginalize_output=True)
             
         else:
             result = self.forward(renormalize=renormalize,
                                   marginalize_output=True)
         
+        if self._n_features == 1:
+            size = result.shape[0]
+            result = result.outer(result).view(size, size)
+        
         return result
     
     @torch.no_grad()
     def entropy(self,
                 middle_site: int,
                 renormalize: bool = False) -> Union[float, Tuple[float]]:
         r"""
@@ -1493,44 +1616,38 @@
         
         for i in range(middle_site):
             result1, result2 = nodes[i]['right'].svd_(
                 side='right',
                 rank=nodes[i]['right'].size())
             
             if renormalize:
-                aux_norm = result2.norm() / sqrt(result2.shape[0])
+                aux_norm = result2.norm()
                 if not aux_norm.isinf() and (aux_norm > 0):
                     result2.tensor = result2.tensor / aux_norm
                     log_norm += aux_norm.log()
 
             result1 = result1.parameterize()
             nodes[i] = result1
             nodes[i + 1] = result2
 
         for i in range(len(nodes) - 1, middle_site, -1):
             result1, result2 = nodes[i]['left'].svd_(
                 side='left',
                 rank=nodes[i]['left'].size())
             
             if renormalize:
-                aux_norm = result1.norm() / sqrt(result1.shape[0])
+                aux_norm = result1.norm()
                 if not aux_norm.isinf() and (aux_norm > 0):
                     result1.tensor = result1.tensor / aux_norm
                     log_norm += aux_norm.log()
 
             result2 = result2.parameterize()
             nodes[i] = result2
             nodes[i - 1] = result1
         
-        if renormalize:
-            aux_norm = nodes[middle_site].norm()
-            if not aux_norm.isinf() and (aux_norm > 0):
-                nodes[middle_site].tensor = nodes[middle_site].tensor / aux_norm
-                log_norm += aux_norm.log()
-        
         nodes[middle_site] = nodes[middle_site].parameterize()
         
         # Compute mutual information
         middle_tensor = nodes[middle_site].tensor.clone()
         _, s, _ = torch.linalg.svd(
             middle_tensor.reshape(middle_tensor.shape[:-1].numel(), # left x input
                                   middle_tensor.shape[-1]),         # right
@@ -1577,14 +1694,19 @@
         equally for all SVD computations.
         
         If none of them are specified, the bond dimensions won't be modified
         if possible. Only when the bond dimension is bigger than the physical
         dimension multiplied by the other bond dimension of the node, it will
         be cropped to that size.
         
+        If rank is not specified, the current bond dimensions will be used as
+        the rank. That is, the current bond dimensions will be the upper bound
+        for the possibly new bond dimensions given by the arguments
+        ``cum_percentage`` and/or ``cutoff``.
+        
         Parameters
         ----------
         oc : int
             Position of the orthogonality center. It should be between 0 and 
             ``n_features - 1``.
         mode : {"svd", "svdr", "qr"}
             Indicates which decomposition should be used to split a node after
@@ -1642,15 +1764,15 @@
                 nodes[0].tensor[1:])
             nodes[-1].tensor[..., 1:] = torch.zeros_like(
                 nodes[-1].tensor[..., 1:])
         
         # If mode is svd or svr and none of the args is provided, the ranks are
         # kept as they were originally
         keep_rank = False
-        if (rank is None) and (cum_percentage is None) and (cutoff is None):
+        if rank is None:
             keep_rank = True
         
         for i in range(oc):
             if mode == 'svd':
                 result1, result2 = nodes[i]['right'].svd_(
                     side='right',
                     rank=nodes[i]['right'].size() if keep_rank else rank,
@@ -1664,15 +1786,15 @@
                     cutoff=cutoff)
             elif mode == 'qr':
                 result1, result2 = nodes[i]['right'].qr_()
             else:
                 raise ValueError('`mode` can only be "svd", "svdr" or "qr"')
             
             if renormalize:
-                aux_norm = result2.norm() / sqrt(result2.shape[0])
+                aux_norm = result2.norm()
                 if not aux_norm.isinf() and (aux_norm > 0):
                     result2.tensor = result2.tensor / aux_norm
                     log_norm += aux_norm.log()
 
             result1 = result1.parameterize()
             nodes[i] = result1
             nodes[i + 1] = result2
@@ -1692,15 +1814,15 @@
                     cutoff=cutoff)
             elif mode == 'qr':
                 result1, result2 = nodes[i]['left'].rq_()
             else:
                 raise ValueError('`mode` can only be "svd", "svdr" or "qr"')
             
             if renormalize:
-                aux_norm = result1.norm() / sqrt(result1.shape[0])
+                aux_norm = result1.norm()
                 if not aux_norm.isinf() and (aux_norm > 0):
                     result1.tensor = result1.tensor / aux_norm
                     log_norm += aux_norm.log()
 
             result2 = result2.parameterize()
             nodes[i] = result2
             nodes[i - 1] = result1
```

### Comparing `tensorkrowch-1.1.1/tensorkrowch/models/mps_data.py` & `tensorkrowch-1.1.2/tensorkrowch/models/mps_data.py`

 * *Files identical despite different names*

### Comparing `tensorkrowch-1.1.1/tensorkrowch/models/peps.py` & `tensorkrowch-1.1.2/tensorkrowch/models/peps.py`

 * *Files identical despite different names*

### Comparing `tensorkrowch-1.1.1/tensorkrowch/models/tree.py` & `tensorkrowch-1.1.2/tensorkrowch/models/tree.py`

 * *Files identical despite different names*

### Comparing `tensorkrowch-1.1.1/tensorkrowch/operations.py` & `tensorkrowch-1.1.2/tensorkrowch/operations.py`

 * *Files 1% similar despite different names*

```diff
@@ -1321,22 +1321,32 @@
             for ax in axis:
                 axis_num.append(node.get_axis_num(ax))
             axis = tuple(axis)
         else:
             axis_num.append(node.get_axis_num(axis))
     
     norm = node.tensor.norm(p=p, dim=axis_num, keepdim=True)
+    norm = torch.where(norm == 0., 1., norm)
     new_tensor = node.tensor / norm
-    new_node = Node._create_resultant(axes_names=node.axes_names,
-                                      name='renormalize',
-                                      network=node._network,
-                                      tensor=new_tensor,
-                                      edges=node._edges,
-                                      node1_list=node.is_node1())
-
+    
+    if isinstance(node, (StackNode, ParamStackNode)):
+        new_node = StackNode._create_resultant(axes_names=node.axes_names,
+                                               name='renormalize',
+                                               network=node._network,
+                                               tensor=new_tensor,
+                                               edges=node._edges,
+                                               node1_list=node.is_node1())
+    else:
+        new_node = Node._create_resultant(axes_names=node.axes_names,
+                                          name='renormalize',
+                                          network=node._network,
+                                          tensor=new_tensor,
+                                          edges=node._edges,
+                                          node1_list=node.is_node1())
+    
     # Create successor
     net = node._network
     args = (node, p, axis)
     successor = Successor(node_ref=node.node_ref(),
                           index=node._tensor_info['index'],
                           child=new_node,
                           hints=axis_num)
@@ -1363,14 +1373,15 @@
     p: Union[int, float] = 2,
     axis: Optional[Union[Ax, Sequence[Ax]]] = None) -> Node:
     
     axis_num = successor.hints
     tensor = node._direct_get_tensor(successor.node_ref,
                                      successor.index)
     norm = tensor.norm(p=p, dim=axis_num, keepdim=True)
+    norm = torch.where(norm == 0., 1., norm)
     new_tensor = tensor / norm
     
     child = successor.child
     child._direct_set_tensor(new_tensor)
 
     # Record in inverse_memory while contracting, if network is traced
     # (to delete memory if possible)
```

### Comparing `tensorkrowch-1.1.1/tensorkrowch/utils.py` & `tensorkrowch-1.1.2/tensorkrowch/utils.py`

 * *Files identical despite different names*

### Comparing `tensorkrowch-1.1.1/tensorkrowch.egg-info/PKG-INFO` & `tensorkrowch-1.1.2/tensorkrowch.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tensorkrowch
-Version: 1.1.1
+Version: 1.1.2
 Summary: Tensor Networks with PyTorch
 Author-email: José Ramón Pareja Monturiol <joserapa98@gmail.com>
 Maintainer-email: José Ramón Pareja Monturiol <joserapa98@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 José Ramón Pareja Monturiol
         
@@ -32,23 +32,26 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: torch>=1.9
 Requires-Dist: opt_einsum>=3.0
 Provides-Extra: tests
 Requires-Dist: pytest; extra == "tests"
+Requires-Dist: pytest-cov; extra == "tests"
 Provides-Extra: docs
 Requires-Dist: sphinx==4.5.0; extra == "docs"
 Requires-Dist: sphinx-book-theme==0.3.3; extra == "docs"
 Requires-Dist: sphinx-copybutton==0.5.2; extra == "docs"
 Requires-Dist: sphinxcontrib-applehelp==1.0.4; extra == "docs"
 Requires-Dist: sphinxcontrib-devhelp==1.0.2; extra == "docs"
 Requires-Dist: sphinxcontrib-htmlhelp==2.0.1; extra == "docs"
 Requires-Dist: sphinxcontrib-qthelp==1.0.3; extra == "docs"
 Requires-Dist: sphinxcontrib-serializinghtml==1.1.5; extra == "docs"
+Requires-Dist: ipykernel; extra == "docs"
+Requires-Dist: nbsphinx==0.9.3; extra == "docs"
 
 ![logo](https://github.com/joserapa98/tensorkrowch/blob/master/docs/figures/svg/tensorkrowch_logo_dark.svg#gh-dark-mode-only)
 ![logo](https://github.com/joserapa98/tensorkrowch/blob/master/docs/figures/svg/tensorkrowch_logo_light.svg#gh-light-mode-only)
 
 [![DOI](https://zenodo.org/badge/453954432.svg)](https://zenodo.org/badge/latestdoi/453954432)
 
 # Tensor Networks with PyTorch
@@ -123,14 +126,20 @@
 
 ```
 python -m pytest -v
 ```
 
 inside the repository folder.
 
+> [!NOTE]
+Certain tests may experience failure as a result of statistical anomalies or 
+hardware constraints. We advise reviewing the error messages to determine if 
+these failures stem from such occurrences. Should this be the case, consider 
+rerunning the tests to ascertain if the errors persist.
+
 
 ## Example
 
 With **TensorKrowch** you can experiment building Tensor Networks:
 
 ```python
 import torch
@@ -200,14 +209,33 @@
 * [Contracting and Differentiating the Tensor Network](https://joserapa98.github.io/tensorkrowch/_build/html/tutorials/2_contracting_tensor_network.html)
 * [How to save Memory and Time with TensorKrowch (ADVANCED)](https://joserapa98.github.io/tensorkrowch/_build/html/tutorials/3_memory_management.html)
 * [The different Types of Nodes (ADVANCED)](https://joserapa98.github.io/tensorkrowch/_build/html/tutorials/4_types_of_nodes.html)
 * [How to subclass TensorNetwork to build Custom Models](https://joserapa98.github.io/tensorkrowch/_build/html/tutorials/5_subclass_tensor_network.html)
 * [Creating a Hybrid Neural-Tensor Network Model](https://joserapa98.github.io/tensorkrowch/_build/html/tutorials/6_mix_with_pytorch.html)
 
 
+## Example Notebooks
+
+In addition to the informative tutorials, there is also a collection of examples
+that serve as practical demonstrations of how to apply **TensorKrowch** in
+various contexts, showcasing its versatility.
+
+With the code provided in the examples, you will be able to reproduce key research
+findings that bridge the gap between tensor networks and machine learning. These
+examples provide a hands-on approach to understanding the intricacies of
+**TensorKrowch**, allowing you to explore its potential and adapt it to your
+specific needs.
+
+* [Training MPS in different ways](https://joserapa98.github.io/tensorkrowch/_build/html/examples/training_mps.html)
+* [Hybrid Tensorial Neural Network model](https://joserapa98.github.io/tensorkrowch/_build/html/examples/hybrid_tnn_model.html)
+* [Tensorizing Neural Networks](https://joserapa98.github.io/tensorkrowch/_build/html/examples/tensorizing_nn.html)
+* [DMRG-like training of MPS](https://joserapa98.github.io/tensorkrowch/_build/html/examples/mps_dmrg.html)
+* [Hybrid DMRG-like training of MPS](https://joserapa98.github.io/tensorkrowch/_build/html/examples/mps_dmrg_hybrid.html)
+
+
 ## License
 
 TensorKrowch is licensed under the MIT License. Please see the [LICENSE](https://github.com/joserapa98/tensorkrowch/blob/master/LICENSE.txt) file for more information.
 
 
 ## Citing
```

### Comparing `tensorkrowch-1.1.1/tensorkrowch.egg-info/SOURCES.txt` & `tensorkrowch-1.1.2/tensorkrowch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

