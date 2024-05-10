# Comparing `tmp/softpy-0.0.4.tar.gz` & `tmp/softpy-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "softpy-0.0.4.tar", last modified: Mon May  6 06:30:41 2024, max compression
+gzip compressed data, was "softpy-0.0.5.tar", last modified: Fri May 10 12:38:00 2024, max compression
```

## Comparing `softpy-0.0.4.tar` & `softpy-0.0.5.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0 andrea    (1000) andrea    (1000)        0 2024-05-06 06:30:41.294910 softpy-0.0.4/
--rwxrwxrwx   0 andrea    (1000) andrea    (1000)      280 2023-03-06 10:54:52.000000 softpy-0.0.4/LICENSE
--rwxrwxrwx   0 andrea    (1000) andrea    (1000)     1019 2024-05-06 06:30:41.296915 softpy-0.0.4/PKG-INFO
--rwxrwxrwx   0 andrea    (1000) andrea    (1000)      715 2024-03-08 13:07:13.000000 softpy-0.0.4/README.md
--rwxrwxrwx   0 andrea    (1000) andrea    (1000)      162 2024-05-06 06:30:41.307911 softpy-0.0.4/setup.cfg
--rwxrwxrwx   0 andrea    (1000) andrea    (1000)      571 2024-05-06 06:29:53.000000 softpy-0.0.4/setup.py
-drwxrwxrwx   0 andrea    (1000) andrea    (1000)        0 2024-05-06 06:30:40.415643 softpy-0.0.4/softpy/
--rwxrwxrwx   0 andrea    (1000) andrea    (1000)       49 2023-05-12 17:24:06.000000 softpy-0.0.4/softpy/__init__.py
-drwxrwxrwx   0 andrea    (1000) andrea    (1000)        0 2024-05-06 06:30:40.962380 softpy-0.0.4/softpy/evolutionary/
--rwxrwxrwx   0 andrea    (1000) andrea    (1000)      708 2024-05-02 10:40:30.000000 softpy-0.0.4/softpy/evolutionary/__init__.py
--rwxrwxrwx   0 andrea    (1000) andrea    (1000)    12572 2023-06-21 10:17:14.000000 softpy-0.0.4/softpy/evolutionary/candidate.py
--rwxrwxrwx   0 andrea    (1000) andrea    (1000)     7558 2024-03-08 14:08:59.000000 softpy-0.0.4/softpy/evolutionary/genetic.py
--rwxrwxrwx   0 andrea    (1000) andrea    (1000)     1285 2023-06-21 10:13:20.000000 softpy-0.0.4/softpy/evolutionary/selection.py
--rwxrwxrwx   0 andrea    (1000) andrea    (1000)     3245 2024-05-06 06:29:19.000000 softpy-0.0.4/softpy/evolutionary/singlestate.py
-drwxrwxrwx   0 andrea    (1000) andrea    (1000)        0 2024-05-06 06:30:41.253556 softpy-0.0.4/softpy/fuzzy/
--rwxrwxrwx   0 andrea    (1000) andrea    (1000)     1336 2024-03-08 14:09:52.000000 softpy-0.0.4/softpy/fuzzy/__init__.py
--rwxrwxrwx   0 andrea    (1000) andrea    (1000)     3254 2024-03-08 14:08:45.000000 softpy-0.0.4/softpy/fuzzy/clustering.py
--rwxrwxrwx   0 andrea    (1000) andrea    (1000)     9634 2024-03-08 14:08:37.000000 softpy-0.0.4/softpy/fuzzy/control.py
--rwxrwxrwx   0 andrea    (1000) andrea    (1000)    20235 2024-03-22 11:48:08.000000 softpy-0.0.4/softpy/fuzzy/fuzzyset.py
--rwxrwxrwx   0 andrea    (1000) andrea    (1000)    14578 2024-03-22 11:52:40.000000 softpy-0.0.4/softpy/fuzzy/operations.py
-drwxrwxrwx   0 andrea    (1000) andrea    (1000)        0 2024-05-06 06:30:40.632445 softpy-0.0.4/softpy.egg-info/
--rwxrwxrwx   0 andrea    (1000) andrea    (1000)     1019 2024-05-06 06:30:39.000000 softpy-0.0.4/softpy.egg-info/PKG-INFO
--rwxrwxrwx   0 andrea    (1000) andrea    (1000)      496 2024-05-06 06:30:40.000000 softpy-0.0.4/softpy.egg-info/SOURCES.txt
--rwxrwxrwx   0 andrea    (1000) andrea    (1000)        1 2024-05-06 06:30:39.000000 softpy-0.0.4/softpy.egg-info/dependency_links.txt
--rwxrwxrwx   0 andrea    (1000) andrea    (1000)       28 2024-05-06 06:30:39.000000 softpy-0.0.4/softpy.egg-info/requires.txt
--rwxrwxrwx   0 andrea    (1000) andrea    (1000)        7 2024-05-06 06:30:39.000000 softpy-0.0.4/softpy.egg-info/top_level.txt
+drwxrwxrwx   0 andrea    (1000) andrea    (1000)        0 2024-05-10 12:38:00.791520 softpy-0.0.5/
+-rwxrwxrwx   0 andrea    (1000) andrea    (1000)      280 2023-03-06 10:54:52.000000 softpy-0.0.5/LICENSE
+-rwxrwxrwx   0 andrea    (1000) andrea    (1000)     1019 2024-05-10 12:38:00.792528 softpy-0.0.5/PKG-INFO
+-rwxrwxrwx   0 andrea    (1000) andrea    (1000)      715 2024-03-08 13:07:13.000000 softpy-0.0.5/README.md
+-rwxrwxrwx   0 andrea    (1000) andrea    (1000)      162 2024-05-10 12:38:00.797530 softpy-0.0.5/setup.cfg
+-rwxrwxrwx   0 andrea    (1000) andrea    (1000)      571 2024-05-10 12:37:32.000000 softpy-0.0.5/setup.py
+drwxrwxrwx   0 andrea    (1000) andrea    (1000)        0 2024-05-10 12:38:00.359595 softpy-0.0.5/softpy/
+-rwxrwxrwx   0 andrea    (1000) andrea    (1000)       49 2023-05-12 17:24:06.000000 softpy-0.0.5/softpy/__init__.py
+drwxrwxrwx   0 andrea    (1000) andrea    (1000)        0 2024-05-10 12:38:00.613448 softpy-0.0.5/softpy/evolutionary/
+-rwxrwxrwx   0 andrea    (1000) andrea    (1000)      708 2024-05-08 13:48:23.000000 softpy-0.0.5/softpy/evolutionary/__init__.py
+-rwxrwxrwx   0 andrea    (1000) andrea    (1000)    14436 2024-05-10 11:12:54.000000 softpy-0.0.5/softpy/evolutionary/candidate.py
+-rwxrwxrwx   0 andrea    (1000) andrea    (1000)     7533 2024-05-10 10:54:28.000000 softpy-0.0.5/softpy/evolutionary/genetic.py
+-rwxrwxrwx   0 andrea    (1000) andrea    (1000)     1285 2023-06-21 10:13:20.000000 softpy-0.0.5/softpy/evolutionary/selection.py
+-rwxrwxrwx   0 andrea    (1000) andrea    (1000)     3245 2024-05-06 06:29:19.000000 softpy-0.0.5/softpy/evolutionary/singlestate.py
+drwxrwxrwx   0 andrea    (1000) andrea    (1000)        0 2024-05-10 12:38:00.771027 softpy-0.0.5/softpy/fuzzy/
+-rwxrwxrwx   0 andrea    (1000) andrea    (1000)     1336 2024-03-08 14:09:52.000000 softpy-0.0.5/softpy/fuzzy/__init__.py
+-rwxrwxrwx   0 andrea    (1000) andrea    (1000)     3242 2024-05-08 13:47:12.000000 softpy-0.0.5/softpy/fuzzy/clustering.py
+-rwxrwxrwx   0 andrea    (1000) andrea    (1000)     9622 2024-05-08 13:47:05.000000 softpy-0.0.5/softpy/fuzzy/control.py
+-rwxrwxrwx   0 andrea    (1000) andrea    (1000)    20235 2024-03-22 11:48:08.000000 softpy-0.0.5/softpy/fuzzy/fuzzyset.py
+-rwxrwxrwx   0 andrea    (1000) andrea    (1000)    14566 2024-05-08 13:46:59.000000 softpy-0.0.5/softpy/fuzzy/operations.py
+drwxrwxrwx   0 andrea    (1000) andrea    (1000)        0 2024-05-10 12:38:00.448711 softpy-0.0.5/softpy.egg-info/
+-rwxrwxrwx   0 andrea    (1000) andrea    (1000)     1019 2024-05-10 12:38:00.000000 softpy-0.0.5/softpy.egg-info/PKG-INFO
+-rwxrwxrwx   0 andrea    (1000) andrea    (1000)      496 2024-05-10 12:38:00.000000 softpy-0.0.5/softpy.egg-info/SOURCES.txt
+-rwxrwxrwx   0 andrea    (1000) andrea    (1000)        1 2024-05-10 12:38:00.000000 softpy-0.0.5/softpy.egg-info/dependency_links.txt
+-rwxrwxrwx   0 andrea    (1000) andrea    (1000)       28 2024-05-10 12:38:00.000000 softpy-0.0.5/softpy.egg-info/requires.txt
+-rwxrwxrwx   0 andrea    (1000) andrea    (1000)        7 2024-05-10 12:38:00.000000 softpy-0.0.5/softpy.egg-info/top_level.txt
```

### Comparing `softpy-0.0.4/PKG-INFO` & `softpy-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: softpy
-Version: 0.0.4
+Version: 0.0.5
 Summary: A package for soft computing in Python.
 Home-page: https://pypi.org/project/scikit-weak/
 Author: Andrea Campagner
 Author-email: onyris93@gmail.com
 License: LICENSE.txt
 Requires-Python: >3.8.0
 Description-Content-Type: text/markdown
```

### Comparing `softpy-0.0.4/README.md` & `softpy-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `softpy-0.0.4/setup.py` & `softpy-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
    name='softpy',
-   version='0.0.4',
+   version='0.0.5',
    author='Andrea Campagner',
    python_requires=">3.8.0",
    author_email='onyris93@gmail.com',
    packages=find_packages(include=['softpy', 'softpy.*']),
    url='https://pypi.org/project/scikit-weak/',
    license='LICENSE.txt',
    description='A package for soft computing in Python.',
```

### Comparing `softpy-0.0.4/softpy/evolutionary/__init__.py` & `softpy-0.0.5/softpy/evolutionary/__init__.py`

 * *Files identical despite different names*

### Comparing `softpy-0.0.4/softpy/evolutionary/candidate.py` & `softpy-0.0.5/softpy/evolutionary/candidate.py`

 * *Files 11% similar despite different names*

```diff
@@ -170,29 +170,31 @@
         def __init__(self, function, children, depth = 1, parent=None, child_id=None):
             self.function = function
             self.children = children
             self.depth = depth
             self.parent = parent
             self.child_id = child_id
 
-    def __init__(self, root: TreeCandidate.NodeCandidate, function_set, arities, max_absolute_depth, constant_generator, stop_early_prob):
+    def __init__(self, root: TreeCandidate.NodeCandidate, function_set, arities, max_absolute_depth, constant_generator, stop_early_prob, mutate_prob):
         self.root = root
         self.function_set = function_set
         self.arities = arities
         self.max_absolute_depth = max_absolute_depth
         self.constant_generator = constant_generator
         self.stop_early_prob = stop_early_prob
+        self.mutate_prob = mutate_prob
 
-    def generate(function_set, arities, max_depth, max_absolute_depth, constant_generator, stop_early_prob = 0.0) -> TreeCandidate:
+    def generate(function_set, arities, max_depth, max_absolute_depth, constant_generator, stop_early_prob = 0.0, mutate_prob=0.2) -> TreeCandidate:
         depth = 1
         parent = None
 
         nodes = []
 
-        if depth >= max_depth:
+        r = np.random.rand()
+        if (depth >= max_depth)  or (r < stop_early_prob):
             val = constant_generator()
             nodes.append(TreeCandidate.NodeCandidate(val, None, depth, parent, None))
         else:
             idx = np.random.choice(range(len(function_set)))
             fun = function_set[idx]
             ari = arities[idx]
             nodes.append(TreeCandidate.NodeCandidate(fun, np.empty(ari, dtype=TreeCandidate.NodeCandidate), depth, parent, None))
@@ -214,31 +216,56 @@
                     fun = function_set[idx]
                     ari = arities[idx]
                     child = TreeCandidate.NodeCandidate(fun, np.empty(ari, dtype=TreeCandidate.NodeCandidate), depth+1, node, i)
                     nodes.append(child)
 
                 node.children[i] = child
 
-        return TreeCandidate(root, function_set, arities, max_absolute_depth, constant_generator, stop_early_prob)
+        return TreeCandidate(root, function_set, arities, max_absolute_depth, constant_generator, stop_early_prob, mutate_prob)
 
 
     def mutate(self) -> TreeCandidate:
         new_tree = deepcopy(self)
         nodes = [new_tree.root]
         while len(nodes) != 0:
             node: TreeCandidate.NodeCandidate = nodes.pop()
             r = np.random.rand()
             if node.depth == new_tree.max_absolute_depth or r < new_tree.stop_early_prob:
                 node.function = new_tree.constant_generator()
                 node.children = None
             else:
-                num = 0 if node.children is None else len(node.children)
-                for i in range(num):
-                    nodes.append(node.children[i])
-
+                r = np.random.rand()
+                if r < new_tree.mutate_prob:
+                    idx = np.random.choice(range(len(new_tree.function_set)))
+                    node.function = new_tree.function_set[idx]
+                    ari = new_tree.arities[idx]
+                    node.children = np.empty(ari, dtype=TreeCandidate.NodeCandidate)
+                    curr_nodes = [node]
+
+                    while len(curr_nodes) != 0:
+                        curr_node: TreeCandidate.NodeCandidate = curr_nodes.pop()
+                        num = 0 if curr_node.children is None else len(curr_node.children)
+                        curr_depth = curr_node.depth
+                        for i in range(num):
+                            r = np.random.rand()
+                            if (curr_depth + 1 == new_tree.max_absolute_depth) or (r < new_tree.stop_early_prob):
+                                val = new_tree.constant_generator()
+                                child = TreeCandidate.NodeCandidate(val, None, curr_depth+1, curr_node, i)
+                            elif curr_depth + 1 < new_tree.max_absolute_depth:
+                                idx = np.random.choice(range(len(new_tree.function_set)))
+                                fun = new_tree.function_set[idx]
+                                ari = new_tree.arities[idx]
+                                child = TreeCandidate.NodeCandidate(fun, np.empty(ari, dtype=TreeCandidate.NodeCandidate), curr_depth+1, curr_node, i)
+                                curr_nodes.append(child)
+
+                            curr_node.children[i] = child
+                else:
+                    num = 0 if node.children is None else len(node.children)
+                    for i in range(num):
+                        nodes.append(node.children[i])
         return new_tree
 
 
     def recombine(self, c: TreeCandidate) -> TreeCandidate:
         rec_tree = deepcopy(self)
         nodes_self = []
         queue_self = [rec_tree.root]
@@ -267,14 +294,17 @@
 
         parent_old : TreeCandidate.NodeCandidate = old.parent
         idx = old.child_id
         depth = old.depth
 
         if parent_old is not None:
             parent_old.children[idx] = new
+        else:
+            rec_tree.root = new
+
         new.parent = parent_old
         new.child_id = idx
         new.depth = depth
         nodes = [new]
         while len(nodes) != 0:
             node: TreeCandidate.NodeCandidate = nodes.pop()
             num = 0 if node.children is None else len(node.children)
```

### Comparing `softpy-0.0.4/softpy/evolutionary/genetic.py` & `softpy-0.0.5/softpy/evolutionary/genetic.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
 import numpy as np
-from softpy.evolutionary.singlestate import MetaHeuristicsAlgorithm
+from .singlestate import MetaHeuristicsAlgorithm
 
 class GeneticAlgorithm(MetaHeuristicsAlgorithm):
     '''
     A generic implementation of an evolutionary algorithm. It supports different individual candidates' representation formats and can thus be used to
     implement the traditional genetic algorithm as well as variants such as genetic programming. It requires specification of the selection and fitness
     function, of the population size as well as whether the algorithm should apply elitism (and with how many elite individuals) or not.
     The **kwargs argument is used to provide additional arguments for individual candidates' initialization.
@@ -32,19 +32,19 @@
 
         self.population = np.array([self.candidate_type.generate(**self.kwargs) for i in range(self.pop_size)])
         self.fitness = np.zeros(self.population.shape)
         self.best = None
         self.fitness_best = np.NINF
 
         if keep_history:
-            self.best_h = np.empty(n_iters+1, dtype=self.candidate_type)
-            self.fitness_h = np.zeros(n_iters+1)
+            self.best_h = np.empty(n_iters, dtype=self.candidate_type)
+            self.fitness_h = np.zeros(n_iters)
             self.fitness_h[:] = np.NINF
 
-        for it in range(n_iters+1):
+        for it in range(n_iters):
             if show_iters:
                 print(it)
             self.fitness = np.vectorize(self.fitness_func)(self.population)
             v = np.max(self.fitness)
             self.best = self.population[np.argmax(self.fitness)] if v > self.fitness_best else self.best
             self.fitness_best = v if v > self.fitness_best else self.fitness_best
```

### Comparing `softpy-0.0.4/softpy/evolutionary/selection.py` & `softpy-0.0.5/softpy/evolutionary/selection.py`

 * *Files identical despite different names*

### Comparing `softpy-0.0.4/softpy/evolutionary/singlestate.py` & `softpy-0.0.5/softpy/evolutionary/singlestate.py`

 * *Files identical despite different names*

### Comparing `softpy-0.0.4/softpy/fuzzy/__init__.py` & `softpy-0.0.5/softpy/fuzzy/__init__.py`

 * *Files identical despite different names*

### Comparing `softpy-0.0.4/softpy/fuzzy/clustering.py` & `softpy-0.0.5/softpy/fuzzy/clustering.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from sklearn.metrics import pairwise_distances
 import numpy as np
 from sklearn.utils import resample
 from sklearn.base import BaseEstimator, ClusterMixin
-from softpy.fuzzy.fuzzyset import DiscreteFuzzySet
+from .fuzzyset import DiscreteFuzzySet
 
 class FuzzyCMeans(BaseEstimator,ClusterMixin):
   '''
   Implements the fuzzy c-means algorithm. The interface is compatible with the scikit-learn library. It allows to set the number of clusters,
   a tolerance degree (for avoiding errors in numerical operations), the number of iterations before termination, the clustering metric as well
   as the fuzzifier degree.
   '''
```

### Comparing `softpy-0.0.4/softpy/fuzzy/control.py` & `softpy-0.0.5/softpy/fuzzy/control.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
 import numpy as np
-from softpy.fuzzy.fuzzyset import FuzzySet, LambdaFuzzySet, DiscreteFuzzySet, ContinuousFuzzySet
+from .fuzzyset import FuzzySet, LambdaFuzzySet, DiscreteFuzzySet, ContinuousFuzzySet
 from abc import ABC, abstractmethod
 from collections.abc import Sequence
 from functools import partial
 import scipy as sp
```

### Comparing `softpy-0.0.4/softpy/fuzzy/fuzzyset.py` & `softpy-0.0.5/softpy/fuzzy/fuzzyset.py`

 * *Files identical despite different names*

### Comparing `softpy-0.0.4/softpy/fuzzy/operations.py` & `softpy-0.0.5/softpy/fuzzy/operations.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
 import numpy as np
-from softpy.fuzzy.fuzzyset import FuzzySet,  DiscreteFuzzySet, ContinuousFuzzySet
+from .fuzzyset import FuzzySet,  DiscreteFuzzySet, ContinuousFuzzySet
 from collections.abc import Sequence
 
 class FuzzyCombination(FuzzySet):
     '''
     Support class to implement a generic combination operator on FuzzySet instances.
     '''
     def __init__(self, left: FuzzySet, right: FuzzySet, op=None):
```

### Comparing `softpy-0.0.4/softpy.egg-info/PKG-INFO` & `softpy-0.0.5/softpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: softpy
-Version: 0.0.4
+Version: 0.0.5
 Summary: A package for soft computing in Python.
 Home-page: https://pypi.org/project/scikit-weak/
 Author: Andrea Campagner
 Author-email: onyris93@gmail.com
 License: LICENSE.txt
 Requires-Python: >3.8.0
 Description-Content-Type: text/markdown
```

