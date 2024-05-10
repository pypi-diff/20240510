# Comparing `tmp/pyxlstm-1.0.0.tar.gz` & `tmp/pyxlstm-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyxlstm-1.0.0.tar", last modified: Fri May 10 06:14:34 2024, max compression
+gzip compressed data, was "pyxlstm-1.0.1.tar", last modified: Fri May 10 07:50:22 2024, max compression
```

## Comparing `pyxlstm-1.0.0.tar` & `pyxlstm-1.0.1.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 mudit      (501) staff       (20)        0 2024-05-10 06:14:34.308952 pyxlstm-1.0.0/
--rw-r--r--   0 mudit      (501) staff       (20)     1071 2024-05-08 20:39:46.000000 pyxlstm-1.0.0/LICENSE
--rw-r--r--   0 mudit      (501) staff       (20)      265 2024-05-09 19:57:59.000000 pyxlstm-1.0.0/MANIFEST.in
--rw-r--r--   0 mudit      (501) staff       (20)    12217 2024-05-10 06:14:34.308596 pyxlstm-1.0.0/PKG-INFO
-drwxr-xr-x   0 mudit      (501) staff       (20)        0 2024-05-10 06:14:34.308303 pyxlstm-1.0.0/PyxLSTM.egg-info/
--rw-r--r--   0 mudit      (501) staff       (20)    12217 2024-05-10 06:14:34.000000 pyxlstm-1.0.0/PyxLSTM.egg-info/PKG-INFO
--rw-r--r--   0 mudit      (501) staff       (20)      587 2024-05-10 06:14:34.000000 pyxlstm-1.0.0/PyxLSTM.egg-info/SOURCES.txt
--rw-r--r--   0 mudit      (501) staff       (20)        1 2024-05-10 06:14:34.000000 pyxlstm-1.0.0/PyxLSTM.egg-info/dependency_links.txt
--rw-r--r--   0 mudit      (501) staff       (20)       42 2024-05-10 06:14:34.000000 pyxlstm-1.0.0/PyxLSTM.egg-info/requires.txt
--rw-r--r--   0 mudit      (501) staff       (20)        6 2024-05-10 06:14:34.000000 pyxlstm-1.0.0/PyxLSTM.egg-info/top_level.txt
--rw-r--r--   0 mudit      (501) staff       (20)     9765 2024-05-10 04:24:15.000000 pyxlstm-1.0.0/README.md
-drwxr-xr-x   0 mudit      (501) staff       (20)        0 2024-05-10 06:14:34.302729 pyxlstm-1.0.0/data/
--rw-r--r--   0 mudit      (501) staff       (20)      864 2024-05-08 20:51:38.000000 pyxlstm-1.0.0/data/dataset.py
--rw-r--r--   0 mudit      (501) staff       (20)     1340 2024-05-08 20:51:51.000000 pyxlstm-1.0.0/data/tokenizer.py
-drwxr-xr-x   0 mudit      (501) staff       (20)        0 2024-05-10 06:14:34.303625 pyxlstm-1.0.0/docs/
--rw-r--r--   0 mudit      (501) staff       (20)     2856 2024-05-10 04:28:03.000000 pyxlstm-1.0.0/docs/mlstm.md
--rw-r--r--   0 mudit      (501) staff       (20)     2691 2024-05-09 04:40:06.000000 pyxlstm-1.0.0/docs/slstm.md
--rw-r--r--   0 mudit      (501) staff       (20)     3533 2024-05-09 20:26:29.000000 pyxlstm-1.0.0/docs/training.md
-drwxr-xr-x   0 mudit      (501) staff       (20)        0 2024-05-10 06:14:34.303980 pyxlstm-1.0.0/examples/
--rw-r--r--   0 mudit      (501) staff       (20)     2206 2024-05-08 21:06:02.000000 pyxlstm-1.0.0/examples/language_modeling.py
--rw-r--r--   0 mudit      (501) staff       (20)     1349 2024-05-10 06:14:25.000000 pyxlstm-1.0.0/pyproject.toml
--rw-r--r--   0 mudit      (501) staff       (20)       18 2024-05-08 21:01:32.000000 pyxlstm-1.0.0/requirements.txt
-drwxr-xr-x   0 mudit      (501) staff       (20)        0 2024-05-10 06:14:34.304947 pyxlstm-1.0.0/scripts/
--rw-r--r--   0 mudit      (501) staff       (20)     2661 2024-05-08 20:51:23.000000 pyxlstm-1.0.0/scripts/evaluate.py
--rw-r--r--   0 mudit      (501) staff       (20)     2574 2024-05-08 20:48:03.000000 pyxlstm-1.0.0/scripts/generate.py
--rw-r--r--   0 mudit      (501) staff       (20)     3891 2024-05-08 20:47:18.000000 pyxlstm-1.0.0/scripts/train.py
--rw-r--r--   0 mudit      (501) staff       (20)       38 2024-05-10 06:14:34.308999 pyxlstm-1.0.0/setup.cfg
-drwxr-xr-x   0 mudit      (501) staff       (20)        0 2024-05-10 06:14:34.305997 pyxlstm-1.0.0/tests/
--rw-r--r--   0 mudit      (501) staff       (20)     2184 2024-05-10 00:44:39.000000 pyxlstm-1.0.0/tests/test_block.py
--rw-r--r--   0 mudit      (501) staff       (20)     1478 2024-05-10 01:29:33.000000 pyxlstm-1.0.0/tests/test_mlstm.py
--rw-r--r--   0 mudit      (501) staff       (20)     1538 2024-05-10 00:44:53.000000 pyxlstm-1.0.0/tests/test_model.py
--rw-r--r--   0 mudit      (501) staff       (20)     1460 2024-05-10 01:29:23.000000 pyxlstm-1.0.0/tests/test_slstm.py
-drwxr-xr-x   0 mudit      (501) staff       (20)        0 2024-05-10 06:14:34.306796 pyxlstm-1.0.0/utils/
--rw-r--r--   0 mudit      (501) staff       (20)      286 2024-05-08 20:53:27.000000 pyxlstm-1.0.0/utils/config.py
--rw-r--r--   0 mudit      (501) staff       (20)      482 2024-05-08 20:53:34.000000 pyxlstm-1.0.0/utils/logging.py
--rw-r--r--   0 mudit      (501) staff       (20)      964 2024-05-08 20:59:17.000000 pyxlstm-1.0.0/utils/utils.py
-drwxr-xr-x   0 mudit      (501) staff       (20)        0 2024-05-10 06:14:34.308016 pyxlstm-1.0.0/xLSTM/
--rw-r--r--   0 mudit      (501) staff       (20)      157 2024-05-10 00:42:44.000000 pyxlstm-1.0.0/xLSTM/__init__.py
--rw-r--r--   0 mudit      (501) staff       (20)     2496 2024-05-10 01:07:42.000000 pyxlstm-1.0.0/xLSTM/block.py
--rw-r--r--   0 mudit      (501) staff       (20)     3648 2024-05-10 01:29:10.000000 pyxlstm-1.0.0/xLSTM/mlstm.py
--rw-r--r--   0 mudit      (501) staff       (20)     1874 2024-05-10 01:08:08.000000 pyxlstm-1.0.0/xLSTM/model.py
--rw-r--r--   0 mudit      (501) staff       (20)     2760 2024-05-10 01:29:02.000000 pyxlstm-1.0.0/xLSTM/slstm.py
+drwxr-xr-x   0 mudit      (501) staff       (20)        0 2024-05-10 07:50:22.701457 pyxlstm-1.0.1/
+-rw-r--r--   0 mudit      (501) staff       (20)     1071 2024-05-08 20:39:46.000000 pyxlstm-1.0.1/LICENSE
+-rw-r--r--   0 mudit      (501) staff       (20)      265 2024-05-09 19:57:59.000000 pyxlstm-1.0.1/MANIFEST.in
+-rw-r--r--   0 mudit      (501) staff       (20)    12223 2024-05-10 07:50:22.701195 pyxlstm-1.0.1/PKG-INFO
+drwxr-xr-x   0 mudit      (501) staff       (20)        0 2024-05-10 07:50:22.700849 pyxlstm-1.0.1/PyxLSTM.egg-info/
+-rw-r--r--   0 mudit      (501) staff       (20)    12223 2024-05-10 07:50:22.000000 pyxlstm-1.0.1/PyxLSTM.egg-info/PKG-INFO
+-rw-r--r--   0 mudit      (501) staff       (20)      587 2024-05-10 07:50:22.000000 pyxlstm-1.0.1/PyxLSTM.egg-info/SOURCES.txt
+-rw-r--r--   0 mudit      (501) staff       (20)        1 2024-05-10 07:50:22.000000 pyxlstm-1.0.1/PyxLSTM.egg-info/dependency_links.txt
+-rw-r--r--   0 mudit      (501) staff       (20)       42 2024-05-10 07:50:22.000000 pyxlstm-1.0.1/PyxLSTM.egg-info/requires.txt
+-rw-r--r--   0 mudit      (501) staff       (20)        6 2024-05-10 07:50:22.000000 pyxlstm-1.0.1/PyxLSTM.egg-info/top_level.txt
+-rw-r--r--   0 mudit      (501) staff       (20)     9771 2024-05-10 07:19:37.000000 pyxlstm-1.0.1/README.md
+drwxr-xr-x   0 mudit      (501) staff       (20)        0 2024-05-10 07:50:22.694892 pyxlstm-1.0.1/data/
+-rw-r--r--   0 mudit      (501) staff       (20)      864 2024-05-08 20:51:38.000000 pyxlstm-1.0.1/data/dataset.py
+-rw-r--r--   0 mudit      (501) staff       (20)     1340 2024-05-08 20:51:51.000000 pyxlstm-1.0.1/data/tokenizer.py
+drwxr-xr-x   0 mudit      (501) staff       (20)        0 2024-05-10 07:50:22.695938 pyxlstm-1.0.1/docs/
+-rw-r--r--   0 mudit      (501) staff       (20)     2846 2024-05-10 07:19:10.000000 pyxlstm-1.0.1/docs/mlstm.md
+-rw-r--r--   0 mudit      (501) staff       (20)     2606 2024-05-10 07:19:27.000000 pyxlstm-1.0.1/docs/slstm.md
+-rw-r--r--   0 mudit      (501) staff       (20)     3533 2024-05-10 07:18:18.000000 pyxlstm-1.0.1/docs/training.md
+drwxr-xr-x   0 mudit      (501) staff       (20)        0 2024-05-10 07:50:22.696396 pyxlstm-1.0.1/examples/
+-rw-r--r--   0 mudit      (501) staff       (20)     3491 2024-05-10 07:37:18.000000 pyxlstm-1.0.1/examples/language_modeling.py
+-rw-r--r--   0 mudit      (501) staff       (20)     1349 2024-05-10 07:47:35.000000 pyxlstm-1.0.1/pyproject.toml
+-rw-r--r--   0 mudit      (501) staff       (20)       18 2024-05-08 21:01:32.000000 pyxlstm-1.0.1/requirements.txt
+drwxr-xr-x   0 mudit      (501) staff       (20)        0 2024-05-10 07:50:22.697175 pyxlstm-1.0.1/scripts/
+-rw-r--r--   0 mudit      (501) staff       (20)     2661 2024-05-10 07:44:21.000000 pyxlstm-1.0.1/scripts/evaluate.py
+-rw-r--r--   0 mudit      (501) staff       (20)     2622 2024-05-10 07:44:38.000000 pyxlstm-1.0.1/scripts/generate.py
+-rw-r--r--   0 mudit      (501) staff       (20)     3939 2024-05-10 07:43:59.000000 pyxlstm-1.0.1/scripts/train.py
+-rw-r--r--   0 mudit      (501) staff       (20)       38 2024-05-10 07:50:22.701497 pyxlstm-1.0.1/setup.cfg
+drwxr-xr-x   0 mudit      (501) staff       (20)        0 2024-05-10 07:50:22.698126 pyxlstm-1.0.1/tests/
+-rw-r--r--   0 mudit      (501) staff       (20)     2184 2024-05-10 00:44:39.000000 pyxlstm-1.0.1/tests/test_block.py
+-rw-r--r--   0 mudit      (501) staff       (20)     1478 2024-05-10 01:29:33.000000 pyxlstm-1.0.1/tests/test_mlstm.py
+-rw-r--r--   0 mudit      (501) staff       (20)     1538 2024-05-10 00:44:53.000000 pyxlstm-1.0.1/tests/test_model.py
+-rw-r--r--   0 mudit      (501) staff       (20)     1460 2024-05-10 01:29:23.000000 pyxlstm-1.0.1/tests/test_slstm.py
+drwxr-xr-x   0 mudit      (501) staff       (20)        0 2024-05-10 07:50:22.698895 pyxlstm-1.0.1/utils/
+-rw-r--r--   0 mudit      (501) staff       (20)      286 2024-05-08 20:53:27.000000 pyxlstm-1.0.1/utils/config.py
+-rw-r--r--   0 mudit      (501) staff       (20)      482 2024-05-08 20:53:34.000000 pyxlstm-1.0.1/utils/logging.py
+-rw-r--r--   0 mudit      (501) staff       (20)      964 2024-05-08 20:59:17.000000 pyxlstm-1.0.1/utils/utils.py
+drwxr-xr-x   0 mudit      (501) staff       (20)        0 2024-05-10 07:50:22.700427 pyxlstm-1.0.1/xLSTM/
+-rw-r--r--   0 mudit      (501) staff       (20)      157 2024-05-10 00:42:44.000000 pyxlstm-1.0.1/xLSTM/__init__.py
+-rw-r--r--   0 mudit      (501) staff       (20)     2496 2024-05-10 01:07:42.000000 pyxlstm-1.0.1/xLSTM/block.py
+-rw-r--r--   0 mudit      (501) staff       (20)     3648 2024-05-10 01:29:10.000000 pyxlstm-1.0.1/xLSTM/mlstm.py
+-rw-r--r--   0 mudit      (501) staff       (20)     1874 2024-05-10 01:08:08.000000 pyxlstm-1.0.1/xLSTM/model.py
+-rw-r--r--   0 mudit      (501) staff       (20)     2760 2024-05-10 01:29:02.000000 pyxlstm-1.0.1/xLSTM/slstm.py
```

### Comparing `pyxlstm-1.0.0/LICENSE` & `pyxlstm-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyxlstm-1.0.0/PKG-INFO` & `pyxlstm-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyxLSTM
-Version: 1.0.0
+Version: 1.0.1
 Summary: PyxLSTM: An efficient and extensible implementation of the xLSTM architecture
 Author-email: Mudit Bhargava <muditbhargava666@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Mudit Bhargava
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -148,15 +148,15 @@
 │   ├── mlstm.md
 │   └── training.md
 │
 ├── examples/
 │   └── language_modeling.py
 │
 ├── .gitignore
-├── setup.py
+├── pyproject.toml
 ├── MANIFEST.in
 ├── requirements.txt
 ├── README.md
 └── LICENSE
 ```
 
 - xLSTM/: The main Python package containing the implementation.
```

### Comparing `pyxlstm-1.0.0/PyxLSTM.egg-info/PKG-INFO` & `pyxlstm-1.0.1/PyxLSTM.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyxLSTM
-Version: 1.0.0
+Version: 1.0.1
 Summary: PyxLSTM: An efficient and extensible implementation of the xLSTM architecture
 Author-email: Mudit Bhargava <muditbhargava666@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Mudit Bhargava
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -148,15 +148,15 @@
 │   ├── mlstm.md
 │   └── training.md
 │
 ├── examples/
 │   └── language_modeling.py
 │
 ├── .gitignore
-├── setup.py
+├── pyproject.toml
 ├── MANIFEST.in
 ├── requirements.txt
 ├── README.md
 └── LICENSE
 ```
 
 - xLSTM/: The main Python package containing the implementation.
```

### Comparing `pyxlstm-1.0.0/PyxLSTM.egg-info/SOURCES.txt` & `pyxlstm-1.0.1/PyxLSTM.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyxlstm-1.0.0/README.md` & `pyxlstm-1.0.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -99,15 +99,15 @@
 │   ├── mlstm.md
 │   └── training.md
 │
 ├── examples/
 │   └── language_modeling.py
 │
 ├── .gitignore
-├── setup.py
+├── pyproject.toml
 ├── MANIFEST.in
 ├── requirements.txt
 ├── README.md
 └── LICENSE
 ```
 
 - xLSTM/: The main Python package containing the implementation.
```

### Comparing `pyxlstm-1.0.0/data/dataset.py` & `pyxlstm-1.0.1/data/dataset.py`

 * *Files identical despite different names*

### Comparing `pyxlstm-1.0.0/data/tokenizer.py` & `pyxlstm-1.0.1/data/tokenizer.py`

 * *Files identical despite different names*

### Comparing `pyxlstm-1.0.0/docs/mlstm.md` & `pyxlstm-1.0.1/docs/slstm.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,81 +1,73 @@
-# mLSTM: Matrix Long Short-Term Memory
+# sLSTM: Scalar Long Short-Term Memory
 
-The mLSTM (Matrix Long Short-Term Memory) is a variant of the LSTM architecture that introduces a matrix memory structure and a covariance update rule. It enhances the traditional LSTM by increasing the storage capacity and enabling parallel computation.
+The sLSTM (Scalar Long Short-Term Memory) is a variant of the LSTM architecture that introduces exponential gating and memory mixing. It enhances the traditional LSTM by enabling the model to revise storage decisions and improve performance on tasks requiring state tracking.
 
 ## Architecture
 
-The mLSTM architecture consists of the following components:
+The sLSTM architecture consists of the following components:
 
-- Input Gate (i): Controls the flow of input information into the memory cell.
-- Forget Gate (f): Determines the amount of information to retain or forget from the previous memory cell state.
-- Output Gate (o): Controls the flow of information from the memory cell to the hidden state.
-- Cell State (C): Stores the long-term memory information as a matrix.
-- Key (k) and Value (v): Represent the input information to be stored in the memory matrix.
-- Query (q): Used to retrieve information from the memory matrix.
+- Input Gate ($i$): Controls the flow of input information into the memory cell.
+- Forget Gate ($f$): Determines the amount of information to retain or forget from the previous memory cell state.
+- Output Gate ($o$): Controls the flow of information from the memory cell to the hidden state.
+- Cell State ($c$): Stores the long-term memory information.
+- Hidden State ($h$): Represents the output of the sLSTM at each time step.
 
-The mLSTM replaces the scalar memory cell state with a matrix memory structure (C). The input information is represented as key-value pairs, where the keys are used to update the memory matrix, and the values are stored in the matrix. The query is used to retrieve information from the memory matrix.
+The sLSTM introduces exponential gating for the input and forget gates, which allows for more fine-grained control over the memory updates. It also incorporates memory mixing, where the hidden state from the previous time step is used to modulate the gates and cell state update.
 
 ## Equations
 
-The equations governing the mLSTM are as follows:
+The equations governing the sLSTM are as follows:
 
 - Cell State Update:
-  $C_t = f_t C_{t-1} + i_t v_t k_t^T$
+  $c_t = f_t \odot c_{t-1} + i_t \odot z_t$
 
 - Normalizer State Update:
-  $n_t = f_t n_{t-1} + i_t k_t$
+  $n_t = f_t \odot n_{t-1} + i_t$
 
 - Hidden State Update:
-  $h_t = o_t \odot \frac{C_t q_t}{max\{ |n_t^T q_t|, 1 \}}$
+  $h_t = o_t \odot \tanh(c_t \odot n_t^{-1})$
 
 - Input Gate:
-  $i_t = exp(w_i^T x_t + b_i)$
+  $i_t = \exp(W_i x_t + b_i)$
 
 - Forget Gate:
-  $f_t = sigmoid(w_f^T x_t + b_f)$
+  $f_t = \exp(W_f x_t + b_f)$
 
 - Output Gate:
-  $o_t = sigmoid(W_o x_t + b_o)$
+  $o_t = \sigmoid(W_o h_t + b_o)$
 
-- Key:
-  $k_t = W_k x_t + b_k$
-
-- Value:
-  $v_t = W_v x_t + b_v$
-
-- Query:
-  $q_t = W_q x_t + b_q$
+- Cell Input:
+  $z_t = 0$
 
 where:
-- $x_t$ is the input vector at time step $t$.
-- $W_\ast$ and $w_\ast$ are weight matrices and vectors, respectively.
-- $b_\ast$ are bias vectors.
+- $x_t$ is the input vector at time step $t$
+- $W_*$ are weight matrices
+- $b_*$ are bias vectors
 
-## Parallelization
+## Initialization and Training
 
-One of the key advantages of the mLSTM is its ability to perform parallel computations. The matrix memory structure allows for efficient parallel updates and retrieval of information.
+The sLSTM can be initialized with random weights and biases. The exponential gating allows for stable training, even with large values.
 
-The mLSTM can be implemented using matrix operations, enabling parallelization on hardware accelerators such as GPUs. This makes the mLSTM suitable for large-scale sequence modeling tasks.
+During training, the gradients are computed using backpropagation through time (BPTT). The sLSTM is trained using standard optimization techniques such as stochastic gradient descent (SGD) or Adam.
 
 ## Usage
 
-To use the mLSTM in your project, you can import the `mLSTM` class from the `xLSTM` package:
+To use the sLSTM in your project, you can import the `sLSTM` class from the `xLSTM` package:
 
 ```python
-from xLSTM import mLSTM
+from xLSTM import sLSTM
 
-# Create an mLSTM instance
-mlstm = mLSTM(input_size, hidden_size, num_layers, dropout)
+# Create an sLSTM instance
+slstm = sLSTM(input_size, hidden_size, num_layers, dropout)
 
 # Forward pass
-outputs, hidden_states = mlstm(inputs)
+outputs, hidden_states = slstm(inputs)
 ```
 
-For more details on using the mLSTM, refer to the API documentation and examples.
+For more details on using the sLSTM, refer to the API documentation and examples.
 
 ## References
 
-- Hochreiter, S., & Schmidhuber, J. (1997). Long short-term memory. Neural computation, 9(8), 1735-1780.
-- Graves, A., Wayne, G., & Danihelka, I. (2014). Neural turing machines. arXiv preprint arXiv:1410.5401.
+- Beck, M., Pöppel, K., Spanring, M., Auer, A., Prudnikova, O., Kopp, M., Klambauer, G., Brandstetter, J., & Hochreiter, S. (2024). xLSTM: Extended Long Short-Term Memory. arXiv preprint arXiv:2405.04517.
 
----
+---
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pyxlstm-1.0.0/docs/training.md` & `pyxlstm-1.0.1/docs/training.md`

 * *Files identical despite different names*

### Comparing `pyxlstm-1.0.0/pyproject.toml` & `pyxlstm-1.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "PyxLSTM"
-version = "1.0.0"
+version = "1.0.1"
 authors = [
     { name = "Mudit Bhargava", email = "muditbhargava666@gmail.com" },
 ]
 description = "PyxLSTM: An efficient and extensible implementation of the xLSTM architecture"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
```

### Comparing `pyxlstm-1.0.0/scripts/evaluate.py` & `pyxlstm-1.0.1/scripts/evaluate.py`

 * *Files identical despite different names*

### Comparing `pyxlstm-1.0.0/scripts/generate.py` & `pyxlstm-1.0.1/scripts/generate.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
             input_ids = torch.tensor([[next_token_id]], dtype=torch.long, device=device)
 
     generated_text = tokenizer.decode(generated_ids)
     return generated_text
 
 def main(args):
     set_seed(args.seed)
-    device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
+    device = torch.device("mps" if torch.backends.mps.is_available() else "cuda" if torch.cuda.is_available() else "cpu")
 
     tokenizer = Tokenizer(args.vocab_file)
 
     model = xLSTM(len(tokenizer), args.embedding_size, args.hidden_size,
                   args.num_layers, args.num_blocks, args.dropout, args.bidirectional, args.lstm_type)
     model.to(device)
```

### Comparing `pyxlstm-1.0.0/scripts/train.py` & `pyxlstm-1.0.1/scripts/train.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
             outputs, _ = model(inputs)
             loss = criterion(outputs.view(-1, model.vocab_size), targets.view(-1))
             epoch_loss += loss.item()
     return epoch_loss / len(dataloader)
 
 def main(args):
     set_seed(args.seed)
-    device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
+    device = torch.device("mps" if torch.backends.mps.is_available() else "cuda" if torch.cuda.is_available() else "cpu")
 
     tokenizer = Tokenizer(args.vocab_file)
     train_dataset = Dataset(args.train_data, tokenizer)
     valid_dataset = Dataset(args.valid_data, tokenizer)
     train_dataloader = DataLoader(train_dataset, batch_size=args.batch_size, shuffle=True)
     valid_dataloader = DataLoader(valid_dataset, batch_size=args.batch_size)
```

### Comparing `pyxlstm-1.0.0/tests/test_block.py` & `pyxlstm-1.0.1/tests/test_block.py`

 * *Files identical despite different names*

### Comparing `pyxlstm-1.0.0/tests/test_mlstm.py` & `pyxlstm-1.0.1/tests/test_mlstm.py`

 * *Files identical despite different names*

### Comparing `pyxlstm-1.0.0/tests/test_model.py` & `pyxlstm-1.0.1/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `pyxlstm-1.0.0/tests/test_slstm.py` & `pyxlstm-1.0.1/tests/test_slstm.py`

 * *Files identical despite different names*

### Comparing `pyxlstm-1.0.0/utils/utils.py` & `pyxlstm-1.0.1/utils/utils.py`

 * *Files identical despite different names*

### Comparing `pyxlstm-1.0.0/xLSTM/block.py` & `pyxlstm-1.0.1/xLSTM/block.py`

 * *Files identical despite different names*

### Comparing `pyxlstm-1.0.0/xLSTM/mlstm.py` & `pyxlstm-1.0.1/xLSTM/mlstm.py`

 * *Files identical despite different names*

### Comparing `pyxlstm-1.0.0/xLSTM/model.py` & `pyxlstm-1.0.1/xLSTM/model.py`

 * *Files identical despite different names*

### Comparing `pyxlstm-1.0.0/xLSTM/slstm.py` & `pyxlstm-1.0.1/xLSTM/slstm.py`

 * *Files identical despite different names*

