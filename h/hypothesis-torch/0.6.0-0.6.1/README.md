# Comparing `tmp/hypothesis_torch-0.6.0.tar.gz` & `tmp/hypothesis_torch-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hypothesis_torch-0.6.0.tar", last modified: Thu May  9 03:09:55 2024, max compression
+gzip compressed data, was "hypothesis_torch-0.6.1.tar", last modified: Fri May 10 04:28:23 2024, max compression
```

## Comparing `hypothesis_torch-0.6.0.tar` & `hypothesis_torch-0.6.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 03:09:55.972857 hypothesis_torch-0.6.0/
--rw-r--r--   0 root         (0) root         (0)     1070 2024-05-09 03:09:21.000000 hypothesis_torch-0.6.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     8094 2024-05-09 03:09:55.972857 hypothesis_torch-0.6.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5282 2024-05-09 03:09:21.000000 hypothesis_torch-0.6.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 03:09:55.968857 hypothesis_torch-0.6.0/hypothesis_torch/
--rw-r--r--   0 root         (0) root         (0)     1454 2024-05-09 03:09:52.000000 hypothesis_torch-0.6.0/hypothesis_torch/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1408 2024-05-09 03:09:21.000000 hypothesis_torch-0.6.0/hypothesis_torch/device.py
--rw-r--r--   0 root         (0) root         (0)     2757 2024-05-09 03:09:21.000000 hypothesis_torch-0.6.0/hypothesis_torch/dtype.py
--rw-r--r--   0 root         (0) root         (0)    10784 2024-05-09 03:09:21.000000 hypothesis_torch-0.6.0/hypothesis_torch/huggingface.py
--rw-r--r--   0 root         (0) root         (0)     2841 2024-05-09 03:09:21.000000 hypothesis_torch-0.6.0/hypothesis_torch/inspection_util.py
--rw-r--r--   0 root         (0) root         (0)      735 2024-05-09 03:09:21.000000 hypothesis_torch-0.6.0/hypothesis_torch/layout.py
--rw-r--r--   0 root         (0) root         (0)      846 2024-05-09 03:09:21.000000 hypothesis_torch-0.6.0/hypothesis_torch/memory_format.py
--rw-r--r--   0 root         (0) root         (0)    10530 2024-05-09 03:09:21.000000 hypothesis_torch-0.6.0/hypothesis_torch/module.py
--rw-r--r--   0 root         (0) root         (0)     4586 2024-05-09 03:09:21.000000 hypothesis_torch-0.6.0/hypothesis_torch/optim.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 03:09:21.000000 hypothesis_torch-0.6.0/hypothesis_torch/py.typed
--rw-r--r--   0 root         (0) root         (0)      866 2024-05-09 03:09:21.000000 hypothesis_torch-0.6.0/hypothesis_torch/register_random_torch_state.py
--rw-r--r--   0 root         (0) root         (0)     9464 2024-05-09 03:09:21.000000 hypothesis_torch-0.6.0/hypothesis_torch/tensor.py
--rw-r--r--   0 root         (0) root         (0)     1442 2024-05-09 03:09:21.000000 hypothesis_torch-0.6.0/hypothesis_torch/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 03:09:55.972857 hypothesis_torch-0.6.0/hypothesis_torch.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8094 2024-05-09 03:09:55.000000 hypothesis_torch-0.6.0/hypothesis_torch.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      665 2024-05-09 03:09:55.000000 hypothesis_torch-0.6.0/hypothesis_torch.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-09 03:09:55.000000 hypothesis_torch-0.6.0/hypothesis_torch.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       91 2024-05-09 03:09:55.000000 hypothesis_torch-0.6.0/hypothesis_torch.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       96 2024-05-09 03:09:55.000000 hypothesis_torch-0.6.0/hypothesis_torch.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2024-05-09 03:09:55.000000 hypothesis_torch-0.6.0/hypothesis_torch.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     2215 2024-05-09 03:09:21.000000 hypothesis_torch-0.6.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-09 03:09:55.972857 hypothesis_torch-0.6.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 04:28:23.674590 hypothesis_torch-0.6.1/
+-rw-r--r--   0 root         (0) root         (0)     1070 2024-05-10 04:27:46.000000 hypothesis_torch-0.6.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     8449 2024-05-10 04:28:23.674590 hypothesis_torch-0.6.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5282 2024-05-10 04:27:46.000000 hypothesis_torch-0.6.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 04:28:23.670590 hypothesis_torch-0.6.1/hypothesis_torch/
+-rw-r--r--   0 root         (0) root         (0)     2168 2024-05-10 04:28:20.000000 hypothesis_torch-0.6.1/hypothesis_torch/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1408 2024-05-10 04:27:46.000000 hypothesis_torch-0.6.1/hypothesis_torch/device.py
+-rw-r--r--   0 root         (0) root         (0)     2757 2024-05-10 04:27:46.000000 hypothesis_torch-0.6.1/hypothesis_torch/dtype.py
+-rw-r--r--   0 root         (0) root         (0)    11506 2024-05-10 04:27:46.000000 hypothesis_torch-0.6.1/hypothesis_torch/huggingface.py
+-rw-r--r--   0 root         (0) root         (0)     2841 2024-05-10 04:27:46.000000 hypothesis_torch-0.6.1/hypothesis_torch/inspection_util.py
+-rw-r--r--   0 root         (0) root         (0)      735 2024-05-10 04:27:46.000000 hypothesis_torch-0.6.1/hypothesis_torch/layout.py
+-rw-r--r--   0 root         (0) root         (0)      846 2024-05-10 04:27:46.000000 hypothesis_torch-0.6.1/hypothesis_torch/memory_format.py
+-rw-r--r--   0 root         (0) root         (0)    11178 2024-05-10 04:27:46.000000 hypothesis_torch-0.6.1/hypothesis_torch/module.py
+-rw-r--r--   0 root         (0) root         (0)     4586 2024-05-10 04:27:46.000000 hypothesis_torch-0.6.1/hypothesis_torch/optim.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-10 04:27:46.000000 hypothesis_torch-0.6.1/hypothesis_torch/py.typed
+-rw-r--r--   0 root         (0) root         (0)      866 2024-05-10 04:27:46.000000 hypothesis_torch-0.6.1/hypothesis_torch/register_random_torch_state.py
+-rw-r--r--   0 root         (0) root         (0)     9464 2024-05-10 04:27:46.000000 hypothesis_torch-0.6.1/hypothesis_torch/tensor.py
+-rw-r--r--   0 root         (0) root         (0)     1442 2024-05-10 04:27:46.000000 hypothesis_torch-0.6.1/hypothesis_torch/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 04:28:23.674590 hypothesis_torch-0.6.1/hypothesis_torch.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8449 2024-05-10 04:28:23.000000 hypothesis_torch-0.6.1/hypothesis_torch.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      665 2024-05-10 04:28:23.000000 hypothesis_torch-0.6.1/hypothesis_torch.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-10 04:28:23.000000 hypothesis_torch-0.6.1/hypothesis_torch.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       91 2024-05-10 04:28:23.000000 hypothesis_torch-0.6.1/hypothesis_torch.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      246 2024-05-10 04:28:23.000000 hypothesis_torch-0.6.1/hypothesis_torch.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2024-05-10 04:28:23.000000 hypothesis_torch-0.6.1/hypothesis_torch.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     2398 2024-05-10 04:27:46.000000 hypothesis_torch-0.6.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-10 04:28:23.674590 hypothesis_torch-0.6.1/setup.cfg
```

### Comparing `hypothesis_torch-0.6.0/LICENSE` & `hypothesis_torch-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hypothesis_torch-0.6.0/PKG-INFO` & `hypothesis_torch-0.6.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hypothesis-torch
-Version: 0.6.0
+Version: 0.6.1
 Summary: Hypothesis strategies for various Pytorch structures, including tensors and modules.
 Author-email: "Andrew P. Sansom" <andrew@euleriancircuit.com>
 License: MIT License
         
         Copyright (c) 2024 Andrew Sansom
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -49,14 +49,21 @@
 Requires-Dist: torch
 Provides-Extra: huggingface
 Requires-Dist: transformers; extra == "huggingface"
 Provides-Extra: dev
 Requires-Dist: ruff==0.4.3; extra == "dev"
 Requires-Dist: pytest==8.2.0; extra == "dev"
 Requires-Dist: pytest-cov==5.0.0; extra == "dev"
+Provides-Extra: docs
+Requires-Dist: mkdocs==1.6.0; extra == "docs"
+Requires-Dist: mkdocstrings[python]==0.25.1; extra == "docs"
+Requires-Dist: mkdocs-autolinks-plugin==0.7.1; extra == "docs"
+Requires-Dist: mkdocs-material==9.4.6; extra == "docs"
+Requires-Dist: mkdocs-snippets==1.3.0; extra == "docs"
+Requires-Dist: mkdocs-exclude==1.0.2; extra == "docs"
 
 # hypothesis-torch
 Hypothesis strategies for various Pytorch structures (including tensors and modules).
 
 [Hypothesis](https://hypothesis.readthedocs.io/en/latest/) is a powerful property-based testing library for Python. It
 lacks built-in support for Pytorch tensors and modules, so this library provides strategies for generating them.
```

### Comparing `hypothesis_torch-0.6.0/README.md` & `hypothesis_torch-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `hypothesis_torch-0.6.0/hypothesis_torch/__init__.py` & `hypothesis_torch-0.6.1/hypothesis_torch/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Hypothesis strategies for various Pytorch structures (including tensors and modules).
 
 [Hypothesis](https://hypothesis.readthedocs.io/en/latest/) is a powerful property-based testing library for Python. It
 lacks built-in support for Pytorch tensors and modules, so this library provides strategies for generating them.
 """
 
-__version__ = "0.6.0"
+__version__ = "0.6.1"
 import importlib.util
 
 from hypothesis_torch.device import (
     device_strategy,
     AVAILABLE_CPU_DEVICES,
     AVAILABLE_CUDA_DEVICES,
     AVAILABLE_MPS_DEVICES,
@@ -28,11 +28,38 @@
 from hypothesis_torch.layout import layout_strategy
 from hypothesis_torch.memory_format import memory_format_strategy
 from hypothesis_torch.module import linear_network_strategy, same_shape_activation_strategy
 from hypothesis_torch.optim import optimizer_strategy, optimizer_type_strategy, OptimizerConstructorWithOnlyParameters
 from hypothesis_torch.register_random_torch_state import TORCH_RANDOM_WRAPPER
 from hypothesis_torch.tensor import tensor_strategy
 
+__all__ = [
+    "device_strategy",
+    "dtype_strategy",
+    "layout_strategy",
+    "memory_format_strategy",
+    "linear_network_strategy",
+    "same_shape_activation_strategy",
+    "optimizer_strategy",
+    "optimizer_type_strategy",
+    "OptimizerConstructorWithOnlyParameters",
+    "tensor_strategy",
+    "TORCH_RANDOM_WRAPPER",
+    "AVAILABLE_CPU_DEVICES",
+    "AVAILABLE_CUDA_DEVICES",
+    "AVAILABLE_MPS_DEVICES",
+    "AVAILABLE_META_DEVICES",
+    "AVAILABLE_PHYSICAL_DEVICES",
+    "FLOAT_DTYPES",
+    "INT_DTYPES",
+    "SIGNED_INT_DTYPES",
+    "UNSIGNED_INT_DTYPES",
+    "COMPLEX_DTYPES",
+    "BOOL_DTYPES",
+    "ALL_DTYPES",
+]
 
 if importlib.util.find_spec("transformers") is not None:
     # Import Hugging Face strategies if transformers is installed
     from hypothesis_torch.huggingface import transformer_strategy, OFFICIALLY_SUPPORTED_TRANSFORMERS
+
+    __all__ += ["transformer_strategy", "OFFICIALLY_SUPPORTED_TRANSFORMERS"]
```

### Comparing `hypothesis_torch-0.6.0/hypothesis_torch/device.py` & `hypothesis_torch-0.6.1/hypothesis_torch/device.py`

 * *Files identical despite different names*

### Comparing `hypothesis_torch-0.6.0/hypothesis_torch/dtype.py` & `hypothesis_torch-0.6.1/hypothesis_torch/dtype.py`

 * *Files identical despite different names*

### Comparing `hypothesis_torch-0.6.0/hypothesis_torch/huggingface.py` & `hypothesis_torch-0.6.1/hypothesis_torch/huggingface.py`

 * *Files 9% similar despite different names*

```diff
@@ -229,17 +229,31 @@
         cls: The transformer class to generate.
         instantiate_weights: Whether to instantiate the weights of the transformer. If False, the transformer will be
             instantiated on the meta device. This is useful for testing uses of transformers models that do not require
             a forward pass.
         kwargs: Keyword arguments to pass to the transformer constructor. If a keyword argument is a strategy, it will
             be drawn from.
 
+    Raises:
+        ValueError: If `instantiate_weights==False` on PyTorch<2, because the torch meta device cannot be used as a
+            context manager.
+
     Returns:
         A strategy for generating Hugging Face transformers.
     """
+    # TODO: Find a way to instantiate weights on the meta device in PyTorch<2.
+    if not hasattr(torch.device("meta"), "__enter__"):  # pragma: no cover
+        if instantiate_weights is False:
+            raise ValueError(
+                "Cannot instantiate weights on the meta device if the meta device context manager is not available.\n"
+                "Please upgrade to PyTorch 2.0.0 or later."
+            )
+        if isinstance(instantiate_weights, st.SearchStrategy):
+            instantiate_weights = instantiate_weights.filter(lambda x: x is True)
+
     if isinstance(cls, st.SearchStrategy):
         cls = draw(cls)
 
     if cls not in OFFICIALLY_SUPPORTED_TRANSFORMERS:
         hypothesis.note(_PLEASE_REPORT_ERROR.format(cls=cls))
 
     assert issubclass(cls, transformers.PreTrainedModel)
```

### Comparing `hypothesis_torch-0.6.0/hypothesis_torch/inspection_util.py` & `hypothesis_torch-0.6.1/hypothesis_torch/inspection_util.py`

 * *Files identical despite different names*

### Comparing `hypothesis_torch-0.6.0/hypothesis_torch/layout.py` & `hypothesis_torch-0.6.1/hypothesis_torch/layout.py`

 * *Files identical despite different names*

### Comparing `hypothesis_torch-0.6.0/hypothesis_torch/memory_format.py` & `hypothesis_torch-0.6.1/hypothesis_torch/memory_format.py`

 * *Files identical despite different names*

### Comparing `hypothesis_torch-0.6.0/hypothesis_torch/module.py` & `hypothesis_torch-0.6.1/hypothesis_torch/module.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Strategies for generating PyTorch Modules."""
 
 from __future__ import annotations
 
+import contextlib
 from typing import TypeVar, Sequence, Mapping
 
 from hypothesis_torch import inspection_util
 import torch
 from hypothesis import strategies as st
 from torch import nn
 
@@ -26,14 +27,30 @@
     allow_nan=False,
     allow_infinity=False,
     allow_subnormal=False,
 )
 POSITIVE_INTS = st.integers(min_value=1)
 
 
+def _context_manager(device: torch.device) -> torch.device | contextlib.nullcontext:
+    """Return a context manager for the device.
+
+    For torch>=2, this is a no-op. The default device will bet set to the `device` inside the returned context.
+    For torch<2, however, this returns an empty context manager. No default device will be set. Consequently, manual
+    casting will be necessary at the end of the context.
+
+    Args:
+        device: The device to use.
+
+    Returns:
+        A context manager for the device.
+    """
+    return device if hasattr(device, "__enter__") else contextlib.nullcontext()
+
+
 @st.composite
 def lower_upper_strategy(draw: st.DrawFn) -> tuple[float, float]:
     """Strategy for generating a pair of floats where the first is less than the second.
 
     Args:
         draw: The draw function provided by `hypothesis`.
 
@@ -205,15 +222,15 @@
         )
 
     if not isinstance(hidden_layer_size, st.SearchStrategy):
         hidden_layer_size = st.just(hidden_layer_size)
     if isinstance(num_hidden_layers, st.SearchStrategy):
         num_hidden_layers = draw(num_hidden_layers)
 
-    with device:
+    with _context_manager(device):
         interior_layer_sizes = draw(
             st.lists(
                 hidden_layer_size,
                 min_size=num_hidden_layers,
                 max_size=num_hidden_layers,
             )
         )
```

### Comparing `hypothesis_torch-0.6.0/hypothesis_torch/optim.py` & `hypothesis_torch-0.6.1/hypothesis_torch/optim.py`

 * *Files identical despite different names*

### Comparing `hypothesis_torch-0.6.0/hypothesis_torch/register_random_torch_state.py` & `hypothesis_torch-0.6.1/hypothesis_torch/register_random_torch_state.py`

 * *Files identical despite different names*

### Comparing `hypothesis_torch-0.6.0/hypothesis_torch/tensor.py` & `hypothesis_torch-0.6.1/hypothesis_torch/tensor.py`

 * *Files identical despite different names*

### Comparing `hypothesis_torch-0.6.0/hypothesis_torch/utils.py` & `hypothesis_torch-0.6.1/hypothesis_torch/utils.py`

 * *Files identical despite different names*

### Comparing `hypothesis_torch-0.6.0/hypothesis_torch.egg-info/PKG-INFO` & `hypothesis_torch-0.6.1/hypothesis_torch.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hypothesis-torch
-Version: 0.6.0
+Version: 0.6.1
 Summary: Hypothesis strategies for various Pytorch structures, including tensors and modules.
 Author-email: "Andrew P. Sansom" <andrew@euleriancircuit.com>
 License: MIT License
         
         Copyright (c) 2024 Andrew Sansom
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -49,14 +49,21 @@
 Requires-Dist: torch
 Provides-Extra: huggingface
 Requires-Dist: transformers; extra == "huggingface"
 Provides-Extra: dev
 Requires-Dist: ruff==0.4.3; extra == "dev"
 Requires-Dist: pytest==8.2.0; extra == "dev"
 Requires-Dist: pytest-cov==5.0.0; extra == "dev"
+Provides-Extra: docs
+Requires-Dist: mkdocs==1.6.0; extra == "docs"
+Requires-Dist: mkdocstrings[python]==0.25.1; extra == "docs"
+Requires-Dist: mkdocs-autolinks-plugin==0.7.1; extra == "docs"
+Requires-Dist: mkdocs-material==9.4.6; extra == "docs"
+Requires-Dist: mkdocs-snippets==1.3.0; extra == "docs"
+Requires-Dist: mkdocs-exclude==1.0.2; extra == "docs"
 
 # hypothesis-torch
 Hypothesis strategies for various Pytorch structures (including tensors and modules).
 
 [Hypothesis](https://hypothesis.readthedocs.io/en/latest/) is a powerful property-based testing library for Python. It
 lacks built-in support for Pytorch tensors and modules, so this library provides strategies for generating them.
```

### Comparing `hypothesis_torch-0.6.0/hypothesis_torch.egg-info/SOURCES.txt` & `hypothesis_torch-0.6.1/hypothesis_torch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hypothesis_torch-0.6.0/pyproject.toml` & `hypothesis_torch-0.6.1/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -44,14 +44,22 @@
   "transformers",
 ]
 dev = [
   "ruff==0.4.3",
   "pytest==8.2.0",
   "pytest-cov==5.0.0"
 ]
+docs = [
+  "mkdocs==1.6.0",
+  "mkdocstrings[python]==0.25.1",
+  "mkdocs-autolinks-plugin==0.7.1",
+  "mkdocs-material==9.4.6",
+  "mkdocs-snippets==1.3.0",
+  "mkdocs-exclude==1.0.2",
+]
 
 [project.urls]
 Homepage = "https://github.com/qthequartermasterman/hypothesis-torch"
 Documentation = "https://github.com/qthequartermasterman/hypothesis-torch"
 Repository = "https://github.com/qthequartermasterman/hypothesis-torch.git"
 Issues = "https://github.com/qthequartermasterman/hypothesis-torch/issues"
```

