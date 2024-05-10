# Comparing `tmp/likelihood-1.2.12.tar.gz` & `tmp/likelihood-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "likelihood-1.2.12.tar", last modified: Fri May 10 00:06:41 2024, max compression
+gzip compressed data, was "likelihood-1.2.9.tar", last modified: Wed Apr  3 19:41:38 2024, max compression
```

## Comparing `likelihood-1.2.12.tar` & `likelihood-1.2.9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 00:06:41.585362 likelihood-1.2.12/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-10 00:06:38.000000 likelihood-1.2.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2297 2024-05-10 00:06:41.585362 likelihood-1.2.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-05-10 00:06:38.000000 likelihood-1.2.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 00:06:41.581362 likelihood-1.2.12/likelihood/
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-10 00:06:38.000000 likelihood-1.2.12/likelihood/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 00:06:41.581362 likelihood-1.2.12/likelihood/graph/
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-10 00:06:38.000000 likelihood-1.2.12/likelihood/graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2891 2024-05-10 00:06:38.000000 likelihood-1.2.12/likelihood/graph/graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     8591 2024-05-10 00:06:38.000000 likelihood-1.2.12/likelihood/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 00:06:41.581362 likelihood-1.2.12/likelihood/models/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-10 00:06:38.000000 likelihood-1.2.12/likelihood/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9404 2024-05-10 00:06:38.000000 likelihood-1.2.12/likelihood/models/regression.py
--rw-r--r--   0 runner    (1001) docker     (127)     2960 2024-05-10 00:06:38.000000 likelihood-1.2.12/likelihood/models/simulation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1552 2024-05-10 00:06:38.000000 likelihood-1.2.12/likelihood/models/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 00:06:41.581362 likelihood-1.2.12/likelihood/tools/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-10 00:06:38.000000 likelihood-1.2.12/likelihood/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7415 2024-05-10 00:06:38.000000 likelihood-1.2.12/likelihood/tools/numeric_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)    40078 2024-05-10 00:06:38.000000 likelihood-1.2.12/likelihood/tools/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 00:06:41.585362 likelihood-1.2.12/likelihood.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2297 2024-05-10 00:06:41.000000 likelihood-1.2.12/likelihood.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-05-10 00:06:41.000000 likelihood-1.2.12/likelihood.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 00:06:41.000000 likelihood-1.2.12/likelihood.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-10 00:06:41.000000 likelihood-1.2.12/likelihood.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-10 00:06:41.000000 likelihood-1.2.12/likelihood.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 00:06:41.585362 likelihood-1.2.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-05-10 00:06:38.000000 likelihood-1.2.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:41:38.250659 likelihood-1.2.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-03 19:41:34.000000 likelihood-1.2.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1843 2024-04-03 19:41:38.250659 likelihood-1.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1280 2024-04-03 19:41:34.000000 likelihood-1.2.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:41:38.246659 likelihood-1.2.9/likelihood/
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-03 19:41:35.000000 likelihood-1.2.9/likelihood/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:41:38.246659 likelihood-1.2.9/likelihood/graph/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-03 19:41:35.000000 likelihood-1.2.9/likelihood/graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2082 2024-04-03 19:41:35.000000 likelihood-1.2.9/likelihood/graph/graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8591 2024-04-03 19:41:35.000000 likelihood-1.2.9/likelihood/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:41:38.250659 likelihood-1.2.9/likelihood/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-03 19:41:35.000000 likelihood-1.2.9/likelihood/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9404 2024-04-03 19:41:35.000000 likelihood-1.2.9/likelihood/models/regression.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2960 2024-04-03 19:41:35.000000 likelihood-1.2.9/likelihood/models/simulation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1552 2024-04-03 19:41:35.000000 likelihood-1.2.9/likelihood/models/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:41:38.250659 likelihood-1.2.9/likelihood/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-03 19:41:35.000000 likelihood-1.2.9/likelihood/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3478 2024-04-03 19:41:35.000000 likelihood-1.2.9/likelihood/tools/numeric_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36497 2024-04-03 19:41:35.000000 likelihood-1.2.9/likelihood/tools/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:41:38.250659 likelihood-1.2.9/likelihood.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1843 2024-04-03 19:41:38.000000 likelihood-1.2.9/likelihood.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-04-03 19:41:38.000000 likelihood-1.2.9/likelihood.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 19:41:38.000000 likelihood-1.2.9/likelihood.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-03 19:41:38.000000 likelihood-1.2.9/likelihood.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-03 19:41:38.000000 likelihood-1.2.9/likelihood.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 19:41:38.250659 likelihood-1.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-04-03 19:41:35.000000 likelihood-1.2.9/setup.py
```

### Comparing `likelihood-1.2.12/LICENSE` & `likelihood-1.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `likelihood-1.2.12/README.md` & `likelihood-1.2.9/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 ![likelihood](https://raw.githubusercontent.com/RodolfoFerro/likelihood/main/likelihood.png)
 
 ![GitHub last commit](https://img.shields.io/github/last-commit/jzsmoreno/likelihood?style=for-the-badge)
 ![GitHub repo size](https://img.shields.io/github/repo-size/jzsmoreno/likelihood?style=for-the-badge)
 ![License](https://img.shields.io/github/license/jzsmoreno/likelihood?style=for-the-badge)
 
 <!-- Project description -->
-This repository contains the code to build the [likelihood package](./likelihood/) which contains tools for typical tasks in maintain machine learning models in production and the training of custom models, for more information review our [`documentation`](https://jzsmoreno.github.io/likelihood/).
+This repository contains the code to build the [likelihood package](./likelihood/) which contains tools for typical tasks in [`MLOps`](https://en.wikipedia.org/wiki/MLOps) and training of custom models.
 
 ## Prerequisities
 
 Before you begin, ensure you have met the following requirements:
 
 * You have a _Windows/Linux/Mac_ machine running [Python 3.10+](https://www.python.org/).
 * You have installed the latest versions of [`pip`](https://pip.pypa.io/en/stable/installing/) and [`virtualenv`](https://virtualenv.pypa.io/en/stable/installation/) or `conda` ([Anaconda](https://www.anaconda.com/distribution/)).
```

### Comparing `likelihood-1.2.12/likelihood/graph/graph.py` & `likelihood-1.2.9/likelihood/graph/graph.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-from typing import List
-
-import networkx as nx
 from IPython.display import HTML, display
 from pandas.core.frame import DataFrame
 from pyvis.network import Network
 
 from likelihood.tools import FeatureSelection
 
 
@@ -14,63 +11,40 @@
     def __init__(self, df: DataFrame, n_importances: int, **kwargs):
         self.G = Network(
             notebook=True, cdn_resources="remote", directed=True
         )  # enable interactive visualization in Jupyter Notebooks
         self.df = df
         self.n_importances = n_importances
         super().__init__(**kwargs)
-        self.labels: List[str] = []
 
     def fit(self, **kwargs) -> None:
         """Fit the model according to the given data and parameters."""
         self.get_digraph(self.df, self.n_importances)
         # create a dictionary with the indexes and names of the dataframe
-        self.get_index = dict(zip(self.X.columns, range(len(self.X.columns))))
+        self.get_index = dict(zip(self.df.columns, range(len(self.df.columns))))
         self._make_network()
 
     def _make_network(self) -> None:
         """Create nodes and edges of the network based on feature importance scores"""
         self._add_nodes()
         for i in range(len(self.all_features_imp_graph)):
             node = self.all_features_imp_graph[i][0]
             edges = self.all_features_imp_graph[i][1]
 
             for label, weight in edges:
-                self.G.add_edge(self.get_index[node], self.get_index[label], weight=weight)
+                self.G.add_edge(i, self.get_index[label], weight=weight)
 
     def _add_nodes(self) -> None:
         for i in range(len(self.all_features_imp_graph)):
             node = self.all_features_imp_graph[i][0]
-            self.labels.append(node)
             self.G.add_node(n_id=i, label=node)
 
     def draw(self, name="graph.html", **kwargs) -> None:
         """Display the network using HTML format"""
         spring_length = kwargs["spring_length"] if "spring_length" in kwargs else 500
         node_distance = kwargs["node_distance"] if "node_distance" in kwargs else 100
         self.G.repulsion(node_distance=node_distance, spring_length=spring_length)
         self.G.show_buttons(filter_=["physics"])
         self.G.show(name)
 
         html_file_content = open(name, "r").read()
         display(HTML(html_file_content))
-
-    def pyvis_to_networkx(self):
-        nx_graph = nx.Graph()
-
-        # Adding nodes
-        nodes = [d["id"] for d in self.G.nodes]
-        for node_dic in self.G.nodes:
-            id = node_dic["label"]
-            del node_dic["label"]
-            nx_graph.add_nodes_from([(id, node_dic)])
-        self.node_edge_dict = dict(zip(nodes, self.labels))
-        del nodes
-
-        # Adding edges
-        for edge in self.G.edges:
-            source, target = self.node_edge_dict[edge["from"]], self.node_edge_dict[edge["to"]]
-            del edge["from"]
-            del edge["to"]
-            nx_graph.add_edges_from([(source, target, edge)])
-
-        return nx_graph
```

### Comparing `likelihood-1.2.12/likelihood/main.py` & `likelihood-1.2.9/likelihood/main.py`

 * *Files identical despite different names*

### Comparing `likelihood-1.2.12/likelihood/models/regression.py` & `likelihood-1.2.9/likelihood/models/regression.py`

 * *Files identical despite different names*

### Comparing `likelihood-1.2.12/likelihood/models/simulation.py` & `likelihood-1.2.9/likelihood/models/simulation.py`

 * *Files identical despite different names*

### Comparing `likelihood-1.2.12/likelihood/models/utils.py` & `likelihood-1.2.9/likelihood/models/utils.py`

 * *Files identical despite different names*

### Comparing `likelihood-1.2.12/likelihood/tools/tools.py` & `likelihood-1.2.9/likelihood/tools/tools.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 import math
 import os
 import pickle
-from typing import Callable, Dict, List, Tuple
+from typing import Callable, List, Tuple
 
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
-import yaml
 from numpy import ndarray
 from pandas.core.frame import DataFrame
 
 # -------------------------------------------------------------------------
 
 """
 Data Science from Scratch, Second Edition, by Joel Grus (O'Reilly).Copyright 2019 Joel Grus, 978-1-492-04113-9
@@ -19,185 +18,97 @@
 
 def minibatches(dataset: List, batch_size: int, shuffle: bool = True) -> List:
     """Generates 'batch_size'-sized minibatches from the dataset
 
     Parameters
     ----------
     dataset : `List`
-        The data to be divided into mini-batch.
     batch_size : `int`
-        Specifies the size of each mini-batch.
     shuffle : `bool`
-        If set `True`, the data will be shuffled before dividing it into mini-batches.
 
-    Returns
-    -------
-    `List[List]`
-        A list of lists containing the mini-batches. Each sublist is a separate mini-batch with length `batch_size`.
     """
 
     # start indexes 0, batch_size, 2 * batch_size, ...
     batch_starts = [start for start in range(0, len(dataset), batch_size)]
 
     if shuffle:
         np.random.shuffle(batch_starts)  # shuffle the batches
 
     for start in batch_starts:
         end = start + batch_size
         yield dataset[start:end]
 
 
 def difference_quotient(f: Callable, x: float, h: float) -> Callable:
-    """Calculates the difference quotient of `f` evaluated at `x` and `x + h`
+    """Calculates the difference quotient of 'f' evaluated at x and x + h
 
     Parameters
     ----------
-    `f(x)` : `Callable`
-        function.
+    f(x) : `Callable` function
     x : `float`
-        Independent term.
     h : `float`
-        Step size.
 
     Returns
     -------
-    `(f(x + h) - f(x)) / h` : `float`
-        Difference quotient of `f` evaluated at `x`.
+    `(f(x + h) - f(x)) / h`
 
     """
 
     return (f(x + h) - f(x)) / h
 
 
-def partial_difference_quotient(f: Callable, v: ndarray, i: int, h: float) -> ndarray:
+def partial_difference_quotient(f: Callable, v: ndarray, i: int, h: float):
     """Calculates the partial difference quotient of `f`
 
     Parameters
     ----------
     `f(x0,...,xi-th)` : `Callable` function
-        Function to differentiate.
-    v : `Vector` | `np.array`
-        1D array representing vector `v=(x0,...,xi)`.
+    v : `Vector` or `np.array`
     h : `float`
-        Step size.
 
     Returns
     -------
-    `(f(w) - f(v)) / h` : `np.array`
-        the `i-th` partial difference quotient of `f` at `v`
+    the `i-th` partial difference quotient of `f` at `v`
 
     """
 
     w = [
         v_j + (h if j == i else 0) for j, v_j in enumerate(v)  # add h to just the ith element of v
     ]
     return (f(w) - f(v)) / h
 
 
-def estimate_gradient(f: Callable, v: ndarray, h: float = 1e-4) -> List[ndarray]:
+def estimate_gradient(f: Callable, v: ndarray, h: float = 1e-4):
     """Calculates the gradient of `f` at `v`
 
     Parameters
     ----------
     `f(x0,...,xi-th)` : `Callable` function
-        Function to differentiate.
-    v : `Vector` | `np.array`
-        1D array representing vector `v=(x0,...,xi)`.
+    v : `Vector` or `np.array`
     h : `float`. By default it is set to `1e-4`
-        The step size used to approximate the derivative.
 
-    Returns
-    -------
-    grad_f : `List[np.array]`
-        A list containing the estimated gradients of each component of `f` evaluated at `v`.
     """
     return [partial_difference_quotient(f, v, i, h) for i in range(len(v))]
 
 
 # -------------------------------------------------------------------------
 
 
-def generate_feature_yaml(
-    df: DataFrame, ignore_features: List[str] = None, yaml_string: bool = False
-) -> Dict | str:
-    """
-    Generate a YAML string containing information about ordinal, numeric, and categorical features
-    based on the given DataFrame.
-
-    Parameters
-    ----------
-    df : `pd.DataFrame`
-        The DataFrame containing the data.
-    ignore_features : `List[`str`]`
-        A list of features to ignore.
-    yaml_string : `bool`
-        If `True`, return the result as a YAML formatted string. Otherwise, return it as a dictionary. Default is `False`.
-
-    Returns
-    -------
-    feature_info : `Dict` | `str`
-        A dictionary with four keys ('ordinal_features', 'numeric_features', 'categorical_features', 'ignore_features')
-        mapping to lists of feature names. Or a YAML formatted string if `yaml_string` is `True`.
-    """
-    feature_info = {
-        "ordinal_features": [],
-        "numeric_features": [],
-        "categorical_features": [],
-        "ignore_features": [],
-    }
-
-    for col in df.columns:
-        if ignore_features and col in ignore_features:
-            continue
-
-        if pd.api.types.is_numeric_dtype(df[col]):
-            feature_info["numeric_features"].append(col)
-        elif pd.api.types.is_object_dtype(df[col]) or pd.api.types.is_categorical_dtype(df[col]):
-            feature_info["categorical_features"].append(col)
-        elif pd.api.types.is_integer_dtype(df[col]):
-            feature_info["ordinal_features"].append(col)
-        elif pd.api.types.is_float_dtype(df[col]):
-            feature_info["ordinal_features"].append(col)
-        elif pd.api.types.is_bool_dtype(df[col]):
-            feature_info["ordinal_features"].append(col)
-        else:
-            print(f"Unknown type for feature {col}")
-        feature_info["ignore_features"] = ignore_features
-
-    if yaml_string:
-        return yaml.dump(feature_info, default_flow_style=False)
-    else:
-        return feature_info
-
-
 # a function that calculates the percentage of missing values per column is defined
 def cal_missing_values(df: DataFrame) -> None:
-    """Calculate the percentage of missing (`NaN`/`NaT`) values per column in a dataframe.
-
-    Parameters
-    ----------
-    df : `DataFrame`
-        The input dataframe.
-
-    Returns
-    -------
-    `None`
-        Prints out a table with columns as index and percentages of missing values as data.
-    """
-
     col = df.columns
     print("Total size : ", "{:,}".format(len(df)))
     for i in col:
         print(
             str(i) + " : " f"{(df.isnull().sum()[i]/(df.isnull().sum()[i]+df[i].count()))*100:.2f}%"
         )
 
 
 def calculate_probability(x: ndarray, points: int = 1, cond: bool = True) -> ndarray:
-    """Calculates the probability of the data.
+    """Calculates the probability of the data
 
     Parameters
     ----------
     x : `np.array`
         An array containing the data.
     points : `int`
         An integer value. By default it is set to `1`.
@@ -243,15 +154,15 @@
                 )
     return p
 
 
 def cdf(
     x: ndarray, poly: int = 9, inv: bool = False, plot: bool = False, savename: str = None
 ) -> ndarray:
-    """Calculates the cumulative distribution function of the data.
+    """Calculates the cumulative distribution function of the data
 
     Parameters
     ----------
     x : `np.array`
         An array containing the data.
     poly : `int`
         An integer value. By default it is set to `9`.
@@ -302,15 +213,15 @@
                 plt.savefig(savename, dpi=300)
             plt.show()
 
     return f, cdf_, ox
 
 
 class corr:
-    """Calculates the correlation of the data.
+    """Calculates the correlation of the data
 
     Parameters
     ----------
     x : `np.array`
         An array containing the data.
     y : `np.array`
         An array containing the data.
@@ -337,15 +248,15 @@
         plt.show()
 
     def __call__(self):
         return self.z
 
 
 class autocorr:
-    """Calculates the autocorrelation of the data.
+    """Calculates the autocorrelation of the data
 
     Parameters
     ----------
     x : `np.array`
         An array containing the data.
 
     Returns
@@ -369,15 +280,15 @@
         plt.show()
 
     def __call__(self):
         return self.z
 
 
 def fft_denoise(dataset: ndarray, sigma: float = 0, mode: bool = True) -> Tuple[ndarray, float]:
-    """Performs the noise removal using the Fast Fourier Transform.
+    """Performs the noise removal using the Fast Fourier Transform
 
     Parameters
     ----------
     dataset : `np.array`
         An array containing the noised data.
     sigma : `float`
         A `float` between `0` and `1`. By default it is set to `0`.
@@ -409,25 +320,21 @@
         if mode:
             print(f"The {i+1}-th row of the dataset has been denoised.")
             print(f"The period is {round(period, 4)}")
     return dataset_, period
 
 
 def get_period(dataset: ndarray) -> float:
-    """Calculates the periodicity of a `dataset`.
+    """Calculates the periodicity of a `dataset`
 
-    Parameters
-    ----------
-    dataset : `ndarray`
-        the `dataset` describing the function over which the period is calculated
+    Args:
+        dataset (`ndarray`): the `dataset` describing the function over which the period is calculated
 
-    Returns
-    -------
-    period : `float`
-        period of the function described by the `dataset`
+    Returns:
+        `float`: period of the function described by the `dataset`
     """
     n = dataset.size
     fhat = np.fft.fft(dataset, n)
     freq = (1 / n) * np.arange(n)
     L = np.arange(1, np.floor(n / 2), dtype="int")
     PSD = fhat * np.conj(fhat) / n
     indices = PSD > np.mean(PSD) + np.std(PSD)
@@ -435,30 +342,26 @@
     period = 1 / (2 * freq[L][np.argmax(fhat[L])])
     return period
 
 
 def sigmoide_inv(y: float) -> float:
     """Calculates the inverse of the sigmoid function
 
-    Parameters
-    ----------
-    y : `float`
-        the number to evaluate the function
+    Args:
+        y (`float`): the number to evaluate the function
 
-    Returns
-    -------
-    `float`
-        value of evaluated function
+    Returns:
+        `float`: value of evaluated function
     """
 
     return math.log(y / (1 - y))
 
 
 def sigmoide(x: float) -> float:
-    """The sigmoid function"""
+
     return 1 / (1 + math.exp(-x))
 
 
 class LogisticRegression:
     """class implementing multiple logistic regression"""
 
     __slots__ = ["importance", "X", "y", "w"]
@@ -976,18 +879,14 @@
                         x = np.where(labels == y_true[j])
                         count_mat[i, x[0]] += 1
 
         return count_mat
 
 
 class OneHotEncoder:
-    """
-    Class used to encode categorical variables.
-    It receives an array of integers and returns a binary array using the one-hot encoding method.
-    """
 
     __slots__ = ["x"]
 
     def __init__(self) -> None:
         pass
 
     def encode(self, x: ndarray | list):
@@ -1029,24 +928,19 @@
         self.all_features_imp_graph: List[Tuple] = []
         self.w_dict = dict()
 
     def get_digraph(self, dataset: DataFrame, n_importances: int) -> str:
         """
         Get directed graph showing importance of features.
 
-        Parameters
-        ----------
-        dataset : `DataFrame`
-            Dataset to be used for generating the graph.
-        n_importances : `int`
-            Number of top importances to show in the graph.
+        Args:
+            dataset (`DataFrame`): Dataset to be used for generating the graph.
+            n_importances (`int`): Number of top importances to show in the graph.
 
-        Returns
-        -------
-        `str`
+        Returns:
             A string representation of the directed graph.
         """
         # Assign and clean dataset
         self._load_data(dataset)
 
         curr_dataset = self.X
         columns = list(curr_dataset.columns)
@@ -1163,15 +1057,15 @@
         self.X.replace(" ", np.nan, inplace=True)
         self.X.dropna(inplace=True)
         self.X = self.X.reset_index()
         self.X = self.X.drop(columns=["index"])
 
 
 def check_nan_inf(df: DataFrame) -> DataFrame:
-    """Check for `NaN` and `Inf` values in the `DataFrame`. If any are found removes them."""
+    """Check for `NaN` and `Inf` values in the `DataFrame`. If any are found, raise an error."""
     nan_values = df.isnull().values.any()
     count = np.isinf(df.select_dtypes(include="number")).values.sum()
     print("There are null values : ", nan_values)
     print("It contains " + str(count) + " infinite values")
     if nan_values:
         warning_type = "UserWarning"
         msg = "Some rows may have been deleted due to the existence of nan values."
```

### Comparing `likelihood-1.2.12/setup.py` & `likelihood-1.2.9/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,40 +1,38 @@
 from pathlib import Path
 
 import setuptools
 
-# Parse the requirements.txt file
-with open("requirements.txt", "r") as f:
-    install_requires = f.read().splitlines()
-
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 about = {}
 ROOT_DIR = Path(__file__).resolve().parent
 PACKAGE_DIR = ROOT_DIR / "likelihood"
 with open(PACKAGE_DIR / "VERSION") as f:
     _version = f.read().strip()
     about["__version__"] = _version
 
 setuptools.setup(
-    name="likelihood",
+    name="likelihood",  # Replace with your own username
     version=about["__version__"],
     author="J. A. Moreno-Guerra",
     author_email="jzs.gm27@gmail.com",
     description="A package that performs the maximum likelihood algorithm.",
     py_modules=["likelihood"],
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/jzsmoreno/likelihood/",
     packages=setuptools.find_packages(),
-    install_requires=install_requires,
-    extras_require={
-        "full": ["networkx", "pyvis"],
-    },
+    install_requires=[
+        "numpy<2.0.0",
+        "matplotlib",
+        "corner",
+        "pyvis",
+    ],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires=">=3.10",
 )
```

