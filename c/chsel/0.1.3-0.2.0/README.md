# Comparing `tmp/chsel-0.1.3.tar.gz` & `tmp/chsel-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chsel-0.1.3.tar", last modified: Mon Jul 10 14:23:21 2023, max compression
+gzip compressed data, was "chsel-0.2.0.tar", last modified: Fri May 10 02:37:34 2024, max compression
```

## Comparing `chsel-0.1.3.tar` & `chsel-0.2.0.tar`

### file list

```diff
@@ -1,25 +1,28 @@
-drwxr-xr-x   0 johnsonzhong   (501) staff       (20)        0 2023-07-10 14:23:21.297149 chsel-0.1.3/
--rw-r--r--   0 johnsonzhong   (501) staff       (20)     1075 2023-07-10 09:19:03.000000 chsel-0.1.3/LICENSE.txt
--rw-r--r--   0 johnsonzhong   (501) staff       (20)    13829 2023-07-10 14:23:21.296721 chsel-0.1.3/PKG-INFO
--rw-r--r--   0 johnsonzhong   (501) staff       (20)    11764 2023-07-10 09:19:03.000000 chsel-0.1.3/README.md
--rw-r--r--   0 johnsonzhong   (501) staff       (20)     4222 2023-07-10 09:20:13.000000 chsel-0.1.3/pyproject.toml
--rw-r--r--   0 johnsonzhong   (501) staff       (20)       38 2023-07-10 14:23:21.297265 chsel-0.1.3/setup.cfg
-drwxr-xr-x   0 johnsonzhong   (501) staff       (20)        0 2023-07-10 14:23:21.286989 chsel-0.1.3/src/
-drwxr-xr-x   0 johnsonzhong   (501) staff       (20)        0 2023-07-10 14:23:21.293816 chsel-0.1.3/src/chsel/
--rw-r--r--   0 johnsonzhong   (501) staff       (20)      595 2023-07-10 09:19:03.000000 chsel-0.1.3/src/chsel/__init__.py
--rw-r--r--   0 johnsonzhong   (501) staff       (20)      492 2023-07-10 09:19:03.000000 chsel-0.1.3/src/chsel/conversion.py
--rw-r--r--   0 johnsonzhong   (501) staff       (20)    31816 2023-07-10 09:19:03.000000 chsel-0.1.3/src/chsel/costs.py
--rw-r--r--   0 johnsonzhong   (501) staff       (20)     3783 2023-07-10 09:19:03.000000 chsel-0.1.3/src/chsel/initialization.py
--rw-r--r--   0 johnsonzhong   (501) staff       (20)    12625 2023-07-10 09:19:03.000000 chsel-0.1.3/src/chsel/quality_diversity.py
--rw-r--r--   0 johnsonzhong   (501) staff       (20)     5692 2023-07-10 09:19:03.000000 chsel-0.1.3/src/chsel/registration_util.py
--rw-r--r--   0 johnsonzhong   (501) staff       (20)     9561 2023-07-10 09:19:03.000000 chsel-0.1.3/src/chsel/sgd.py
--rw-r--r--   0 johnsonzhong   (501) staff       (20)      628 2023-07-10 09:19:03.000000 chsel-0.1.3/src/chsel/types.py
--rw-r--r--   0 johnsonzhong   (501) staff       (20)    14488 2023-07-10 09:19:03.000000 chsel-0.1.3/src/chsel/wrapper.py
-drwxr-xr-x   0 johnsonzhong   (501) staff       (20)        0 2023-07-10 14:23:21.295866 chsel-0.1.3/src/chsel.egg-info/
--rw-r--r--   0 johnsonzhong   (501) staff       (20)    13829 2023-07-10 14:23:21.000000 chsel-0.1.3/src/chsel.egg-info/PKG-INFO
--rw-r--r--   0 johnsonzhong   (501) staff       (20)      434 2023-07-10 14:23:21.000000 chsel-0.1.3/src/chsel.egg-info/SOURCES.txt
--rw-r--r--   0 johnsonzhong   (501) staff       (20)        1 2023-07-10 14:23:21.000000 chsel-0.1.3/src/chsel.egg-info/dependency_links.txt
--rw-r--r--   0 johnsonzhong   (501) staff       (20)      112 2023-07-10 14:23:21.000000 chsel-0.1.3/src/chsel.egg-info/requires.txt
--rw-r--r--   0 johnsonzhong   (501) staff       (20)        6 2023-07-10 14:23:21.000000 chsel-0.1.3/src/chsel.egg-info/top_level.txt
-drwxr-xr-x   0 johnsonzhong   (501) staff       (20)        0 2023-07-10 14:23:21.296181 chsel-0.1.3/tests/
--rw-r--r--   0 johnsonzhong   (501) staff       (20)    12205 2023-07-10 14:16:24.000000 chsel-0.1.3/tests/test_wrapper.py
+drwxrwxr-x   0 zhsh      (1002) zhsh      (1002)        0 2024-05-10 02:37:34.185479 chsel-0.2.0/
+-rw-rw-r--   0 zhsh      (1002) zhsh      (1002)     1075 2024-05-01 19:55:51.000000 chsel-0.2.0/LICENSE.txt
+-rw-r--r--   0 zhsh      (1002) zhsh      (1002)    17389 2024-05-10 02:37:34.185479 chsel-0.2.0/PKG-INFO
+-rw-rw-r--   0 zhsh      (1002) zhsh      (1002)    15048 2024-05-10 02:31:36.000000 chsel-0.2.0/README.md
+-rw-rw-r--   0 zhsh      (1002) zhsh      (1002)     4233 2024-05-10 02:32:19.000000 chsel-0.2.0/pyproject.toml
+-rw-rw-r--   0 zhsh      (1002) zhsh      (1002)       38 2024-05-10 02:37:34.185479 chsel-0.2.0/setup.cfg
+drwxrwxr-x   0 zhsh      (1002) zhsh      (1002)        0 2024-05-10 02:37:34.185479 chsel-0.2.0/src/
+drwxrwxr-x   0 zhsh      (1002) zhsh      (1002)        0 2024-05-10 02:37:34.185479 chsel-0.2.0/src/chsel/
+-rw-rw-r--   0 zhsh      (1002) zhsh      (1002)      722 2024-05-10 02:32:08.000000 chsel-0.2.0/src/chsel/__init__.py
+-rw-rw-r--   0 zhsh      (1002) zhsh      (1002)      968 2024-05-01 19:55:51.000000 chsel-0.2.0/src/chsel/conversion.py
+-rw-rw-r--   0 zhsh      (1002) zhsh      (1002)    30904 2024-05-10 02:31:36.000000 chsel-0.2.0/src/chsel/costs.py
+-rw-rw-r--   0 zhsh      (1002) zhsh      (1002)     3946 2024-05-10 02:31:36.000000 chsel-0.2.0/src/chsel/initialization.py
+-rw-rw-r--   0 zhsh      (1002) zhsh      (1002)     5386 2024-05-10 02:31:36.000000 chsel-0.2.0/src/chsel/measure.py
+-rw-rw-r--   0 zhsh      (1002) zhsh      (1002)    13231 2024-05-10 02:32:31.000000 chsel-0.2.0/src/chsel/quality_diversity.py
+-rw-rw-r--   0 zhsh      (1002) zhsh      (1002)     4478 2024-05-10 02:31:36.000000 chsel-0.2.0/src/chsel/registration_util.py
+-rw-rw-r--   0 zhsh      (1002) zhsh      (1002)     3079 2024-05-10 02:31:36.000000 chsel-0.2.0/src/chsel/se2.py
+-rw-rw-r--   0 zhsh      (1002) zhsh      (1002)    12852 2024-05-10 02:31:36.000000 chsel-0.2.0/src/chsel/sgd.py
+-rw-rw-r--   0 zhsh      (1002) zhsh      (1002)      647 2024-05-10 02:31:36.000000 chsel-0.2.0/src/chsel/types.py
+-rw-rw-r--   0 zhsh      (1002) zhsh      (1002)    20912 2024-05-10 02:34:06.000000 chsel-0.2.0/src/chsel/wrapper.py
+drwxrwxr-x   0 zhsh      (1002) zhsh      (1002)        0 2024-05-10 02:37:34.185479 chsel-0.2.0/src/chsel.egg-info/
+-rw-r--r--   0 zhsh      (1002) zhsh      (1002)    17389 2024-05-10 02:37:34.000000 chsel-0.2.0/src/chsel.egg-info/PKG-INFO
+-rw-rw-r--   0 zhsh      (1002) zhsh      (1002)      490 2024-05-10 02:37:34.000000 chsel-0.2.0/src/chsel.egg-info/SOURCES.txt
+-rw-rw-r--   0 zhsh      (1002) zhsh      (1002)        1 2024-05-10 02:37:34.000000 chsel-0.2.0/src/chsel.egg-info/dependency_links.txt
+-rw-rw-r--   0 zhsh      (1002) zhsh      (1002)      116 2024-05-10 02:37:34.000000 chsel-0.2.0/src/chsel.egg-info/requires.txt
+-rw-rw-r--   0 zhsh      (1002) zhsh      (1002)        6 2024-05-10 02:37:34.000000 chsel-0.2.0/src/chsel.egg-info/top_level.txt
+drwxrwxr-x   0 zhsh      (1002) zhsh      (1002)        0 2024-05-10 02:37:34.185479 chsel-0.2.0/tests/
+-rw-rw-r--   0 zhsh      (1002) zhsh      (1002)    14917 2024-05-10 02:31:36.000000 chsel-0.2.0/tests/test_se2.py
+-rw-rw-r--   0 zhsh      (1002) zhsh      (1002)    13295 2024-05-10 02:33:55.000000 chsel-0.2.0/tests/test_wrapper.py
```

### Comparing `chsel-0.1.3/LICENSE.txt` & `chsel-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `chsel-0.1.3/PKG-INFO` & `chsel-0.2.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,48 +1,7 @@
-Metadata-Version: 2.1
-Name: chsel
-Version: 0.1.3
-Summary: Constrained pose Hypothesis Set Elimination official code for pose estimation
-Author-email: Sheng Zhong <zhsh@umich.edu>
-Maintainer-email: Sheng Zhong <zhsh@umich.edu>
-License: Copyright (c) 2023 University of Michigan ARM Lab
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy of
-        this software and associated documentation files (the "Software"), to deal in
-        the Software without restriction, including without limitation the rights to
-        use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
-        of the Software, and to permit persons to whom the Software is furnished to do
-        so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-        SOFTWARE.
-        
-        
-Project-URL: Homepage, https://github.com/UM-ARM-Lab/chsel
-Project-URL: Bug Reports, https://github.com/UM-ARM-Lab/cshel/issues
-Project-URL: Source, https://github.com/UM-ARM-Lab/chsel
-Keywords: robotics,pose estimation,registration,pytorch
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-Provides-Extra: test
-License-File: LICENSE.txt
-
 ## CHSEL: Producing Diverse Plausible Pose Estimates from Contact and Free Space Data
 
 ![combined demo](https://i.imgur.com/T4DnKDu.gif)
 
 Demo CHSEL results on drill with sparse contact data (top) and mug with dense vision data (bottom).
 
 ## Installation
@@ -67,14 +26,39 @@
   year={2023}
 }
 ```
 
 To reproduce the results from the paper, see the 
 [experiments repository](https://github.com/UM-ARM-Lab/chsel_experiments).
 
+## Intuition
+### Cost
+* enforce an object's signed distance field (SDF) consistency against point clouds augmented with volumetric semantics
+    * whether a point is in free space, inside the object, or has a known SDF value 
+* two of those semantics classes encodes uncertainty about the observed point's SDF
+    * for example free space just means we know the point has SDF > 0, but makes no claim about its actual value
+    * in many observation scenarios, we do not know the observed' point's actual SDF value
+* compared to related methods like SDF2SDF that match an SDF against another SDF, this avoids bias
+
+### Optimization
+At a high level, our method can be summarized as:
+1. start with an initial set of transforms that ideally covers all local minima
+   * for every local minima, there exists a transform in the initial set that is in its attraction basin in terms of the local cost landscape
+3. find the bounds of the local minima landscape
+    * usually much smaller than the whole search space
+    * do this by performing gradient descent independently on each initial transform with our given cost
+4. consider search in a dimensionality reduced feature space
+    * translational component of the transform such that we consider the best rotation for each translation
+6. find good local minima with a fine-tuning search with the search space reduced to the local minima bounds that we found to afford higher resolution
+    * instead of finding the best local minima, we want to evaluate all local minima, and we do this with Quality Diversity optimization on the feature space
+    * we maintain an archive, a grid in feature space, each cell of which holds the best solution given that archive (so the grid is in translation space, and each cell holds a full transform)
+    * we populate this archive over the course of QD optimization, which evolutionarily combines the top solutions
+7. we return the transforms from the best scoring cells, as many as requested
+    * usually same number as in the input transform set
+
 ## Usage
 CHSEL registers an observed semantic point cloud against a target object's signed distance field (SDF).
 It is agnostic to how the semantic point cloud is obtained, which can come from cameras and tactile sensors for example.
 
 Example code is given in `tests/test_wrapper.py`.
 
 First you need an object frame SDF which you can generate from its 3D mesh
@@ -325,7 +309,35 @@
 # feed all solutions from the previous iteration
 # assuming the object hasn't moved, use the output of the previous iteration as the initial estimate
 # this res is from the last iteration of the previous registration
 world_to_link = chsel.solution_to_world_to_link_matrix(res)
 res, all_solutions = registration.register(iterations=5, batch=B, initial_tsf=world_to_link,
                                            low_cost_transform_set=all_solutions)
 ```
+
+### SE(2) Constraint
+If you know the object lies on a table top for example, you can constrain the optimization to be over
+SE(2) instead of SE(3). You do this by specifying the plane via the axis of rotation (normal) and a
+scalar offset:
+```python
+# table top assumed to face positive z
+normal = torch.tensor([0, 0, 1])
+offset = torch.tensor([0, 0, 0])
+registration = chsel.CHSEL(sdf, positions, semantics, axis_of_rotation=normal, offset_along_normal=offset)
+```
+
+### Measures
+QD optimization works by binning over the measure space. This is how diversity is enforced.
+You can specify the measure space by providing a `chsel.measure.MeasureFunction` object.
+Note that this also defines what space the QD optimization is performed in. (such as a 9 dimensional continuous 
+representation of SE(3) transforms, or a 3 dimensional space for SE(2) transforms).
+
+For example, if you are on a tabletop and know the object's position quite well and want diversity in yaw:
+
+```python
+import chsel
+
+normal = torch.tensor([0, 0, 1])
+offset = torch.tensor([0, 0, 0])
+measure = chsel.SE2AngleMeasure(axis_of_rotation=normal, offset_along_normal=offset)
+registration = chsel.CHSEL(sdf, positions, semantics, axis_of_rotation=normal, offset_along_normal=offset)
+```
```

### Comparing `chsel-0.1.3/README.md` & `chsel-0.2.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,7 +1,58 @@
+Metadata-Version: 2.1
+Name: chsel
+Version: 0.2.0
+Summary: Constrained pose Hypothesis Set Elimination official code for pose estimation
+Author-email: Sheng Zhong <zhsh@umich.edu>
+Maintainer-email: Sheng Zhong <zhsh@umich.edu>
+License: Copyright (c) 2023 University of Michigan ARM Lab
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy of
+        this software and associated documentation files (the "Software"), to deal in
+        the Software without restriction, including without limitation the rights to
+        use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
+        of the Software, and to permit persons to whom the Software is furnished to do
+        so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+        
+        
+Project-URL: Homepage, https://github.com/UM-ARM-Lab/chsel
+Project-URL: Bug Reports, https://github.com/UM-ARM-Lab/cshel/issues
+Project-URL: Source, https://github.com/UM-ARM-Lab/chsel
+Keywords: robotics,pose estimation,registration,pytorch
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+Requires-Dist: cma
+Requires-Dist: torch
+Requires-Dist: numpy
+Requires-Dist: matplotlib
+Requires-Dist: arm-pytorch-utilities
+Requires-Dist: pytorch-kinematics
+Requires-Dist: pytorch-volumetric
+Requires-Dist: cma
+Requires-Dist: ribs[all]
+Provides-Extra: test
+Requires-Dist: pytest; extra == "test"
+
 ## CHSEL: Producing Diverse Plausible Pose Estimates from Contact and Free Space Data
 
 ![combined demo](https://i.imgur.com/T4DnKDu.gif)
 
 Demo CHSEL results on drill with sparse contact data (top) and mug with dense vision data (bottom).
 
 ## Installation
@@ -26,14 +77,39 @@
   year={2023}
 }
 ```
 
 To reproduce the results from the paper, see the 
 [experiments repository](https://github.com/UM-ARM-Lab/chsel_experiments).
 
+## Intuition
+### Cost
+* enforce an object's signed distance field (SDF) consistency against point clouds augmented with volumetric semantics
+    * whether a point is in free space, inside the object, or has a known SDF value 
+* two of those semantics classes encodes uncertainty about the observed point's SDF
+    * for example free space just means we know the point has SDF > 0, but makes no claim about its actual value
+    * in many observation scenarios, we do not know the observed' point's actual SDF value
+* compared to related methods like SDF2SDF that match an SDF against another SDF, this avoids bias
+
+### Optimization
+At a high level, our method can be summarized as:
+1. start with an initial set of transforms that ideally covers all local minima
+   * for every local minima, there exists a transform in the initial set that is in its attraction basin in terms of the local cost landscape
+3. find the bounds of the local minima landscape
+    * usually much smaller than the whole search space
+    * do this by performing gradient descent independently on each initial transform with our given cost
+4. consider search in a dimensionality reduced feature space
+    * translational component of the transform such that we consider the best rotation for each translation
+6. find good local minima with a fine-tuning search with the search space reduced to the local minima bounds that we found to afford higher resolution
+    * instead of finding the best local minima, we want to evaluate all local minima, and we do this with Quality Diversity optimization on the feature space
+    * we maintain an archive, a grid in feature space, each cell of which holds the best solution given that archive (so the grid is in translation space, and each cell holds a full transform)
+    * we populate this archive over the course of QD optimization, which evolutionarily combines the top solutions
+7. we return the transforms from the best scoring cells, as many as requested
+    * usually same number as in the input transform set
+
 ## Usage
 CHSEL registers an observed semantic point cloud against a target object's signed distance field (SDF).
 It is agnostic to how the semantic point cloud is obtained, which can come from cameras and tactile sensors for example.
 
 Example code is given in `tests/test_wrapper.py`.
 
 First you need an object frame SDF which you can generate from its 3D mesh
@@ -284,7 +360,35 @@
 # feed all solutions from the previous iteration
 # assuming the object hasn't moved, use the output of the previous iteration as the initial estimate
 # this res is from the last iteration of the previous registration
 world_to_link = chsel.solution_to_world_to_link_matrix(res)
 res, all_solutions = registration.register(iterations=5, batch=B, initial_tsf=world_to_link,
                                            low_cost_transform_set=all_solutions)
 ```
+
+### SE(2) Constraint
+If you know the object lies on a table top for example, you can constrain the optimization to be over
+SE(2) instead of SE(3). You do this by specifying the plane via the axis of rotation (normal) and a
+scalar offset:
+```python
+# table top assumed to face positive z
+normal = torch.tensor([0, 0, 1])
+offset = torch.tensor([0, 0, 0])
+registration = chsel.CHSEL(sdf, positions, semantics, axis_of_rotation=normal, offset_along_normal=offset)
+```
+
+### Measures
+QD optimization works by binning over the measure space. This is how diversity is enforced.
+You can specify the measure space by providing a `chsel.measure.MeasureFunction` object.
+Note that this also defines what space the QD optimization is performed in. (such as a 9 dimensional continuous 
+representation of SE(3) transforms, or a 3 dimensional space for SE(2) transforms).
+
+For example, if you are on a tabletop and know the object's position quite well and want diversity in yaw:
+
+```python
+import chsel
+
+normal = torch.tensor([0, 0, 1])
+offset = torch.tensor([0, 0, 0])
+measure = chsel.SE2AngleMeasure(axis_of_rotation=normal, offset_along_normal=offset)
+registration = chsel.CHSEL(sdf, positions, semantics, axis_of_rotation=normal, offset_along_normal=offset)
+```
```

### Comparing `chsel-0.1.3/pyproject.toml` & `chsel-0.2.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [project]
 name = "chsel"
-version = "0.1.3"
+version = "0.2.0"
 description = "Constrained pose Hypothesis Set Elimination official code for pose estimation"
 readme = "README.md" # Optional
 
 # Specify which Python versions you support. In contrast to the
 # 'Programming Language' classifiers above, 'pip install' will check this
 # and refuse to install the project if the version does not match. See
 # https://packaging.python.org/guides/distributing-packages-using-setuptools/#python-requires
-requires-python = ">=3.6"
+requires-python = ">=3.9"
 
 # This is either text indicating the license for the distribution, or a file
 # that contains the license
 # https://packaging.python.org/en/latest/specifications/core-metadata/#license
 license = { file = "LICENSE.txt" }
 
 # This field adds keywords for your project which will appear on the
@@ -48,14 +48,15 @@
 # This field lists other packages that your project depends on to run.
 # Any package you put here will be installed by pip when your project is
 # installed, so they must be valid existing projects.
 #
 # For an analysis of this field vs pip's requirements files see:
 # https://packaging.python.org/discussions/install-requires-vs-requirements/
 dependencies = [# Optional
+    'cma',
     'torch',
     'numpy',
     'matplotlib',
     'arm-pytorch-utilities',
     'pytorch-kinematics',
     'pytorch-volumetric',
     'cma',
```

### Comparing `chsel-0.1.3/src/chsel/__init__.py` & `chsel-0.2.0/src/chsel/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 from chsel.wrapper import CHSEL
 from chsel.types import Semantics, SemanticsClass
 from chsel.registration_util import solution_to_world_to_link_matrix, apply_similarity_transform
 from chsel.costs import VolumetricCost, VolumetricDirectSDFCost, VolumetricDoubleDirectCost
 from chsel.initialization import reinitialize_transform_estimates, random_rotation_perturbations, \
     reinitialize_transform_around_elites
-from chsel.conversion import continuous_representation_to_RT, RT_to_continuous_representation
-from chsel.quality_diversity import rot_measure, position_measure, CMAME, CMAMEGA, CMAES
+from chsel.conversion import continuous_representation_to_RT, RT_to_continuous_representation, \
+    continuous_representation_to_H, H_to_continuous_representation
+from chsel.quality_diversity import CMAME, CMAMEGA, CMAES
+from chsel.measure import MeasureFunction, RotMeasure, PositionMeasure, SE2AngleMeasure
```

### Comparing `chsel-0.1.3/src/chsel/costs.py` & `chsel-0.2.0/src/chsel/costs.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 import matplotlib.colors, matplotlib.cm
 import torch
 import typing
 
 import pytorch_volumetric as pv
 from chsel.registration_util import apply_similarity_transform
 from typing import Any
+import logging
+
+logger = logging.getLogger(__name__)
 
 
 class RegistrationCost:
     def __call__(self, R, T, s, other_info=None):
         """Cost for given pose guesses of ICP
 
         :param R: B x 3 x 3
@@ -88,31 +91,31 @@
         # this full lookup is much, much slower than the cached version with points, but are about equivalent
         sdf_value, sdf_grad = sdf(model_frame_free_pos[violating])
         # interior points will have sdf_value < 0
         loss = torch.zeros(model_frame_free_pos.shape[:-1], dtype=model_frame_free_pos.dtype,
                            device=model_frame_free_pos.device)
         violation = interior_threshold - sdf_value
         loss[violating] = violation
-        loss = loss.sum(dim=-1)
         ctx.save_for_backward(violating, violation, sdf_value, sdf_grad)
+        # returns Batch x Points; sum over dim=-1 to get per transform
         return loss
 
     @staticmethod
     def backward(ctx: Any, grad_outputs: Any) -> Any:
         # need to output the gradient of the loss w.r.t. all the inputs of forward
         dl_dsdf = None
         dl_dvoxels = None
         dl_dthreshold = None
         if ctx.needs_input_grad[1]:
             violating, violation, sdf_value, sdf_grad = ctx.saved_tensors
             # SDF grads point away from the surface; in this case we want to move the surface away from the occupied
             grads = torch.zeros(list(violating.shape) + [3], dtype=grad_outputs.dtype, device=grad_outputs.device)
             # free space point, so the surface needs to go in the opposite direction
             grads[violating] = violation.unsqueeze(-1) * sdf_grad
-            dl_dvoxels = grad_outputs[:, None, None] * -grads
+            dl_dvoxels = grad_outputs[:, :, None] * -grads
 
         # gradients for the other inputs not implemented
         return dl_dsdf, dl_dvoxels, dl_dthreshold
 
 
 class OccupiedLookupCost(torch.autograd.Function):
     @staticmethod
@@ -121,17 +124,16 @@
         interior_threshold = - surface_threshold
         violating = sdf.outside_surface(model_frame_occ_pos, surface_level=surface_threshold)
         # this full lookup is much, much slower than the cached version with points, but are about equivalent
         sdf_value, sdf_grad = sdf(model_frame_occ_pos[violating])
         # interior points will have sdf_value < 0
         loss = torch.zeros(model_frame_occ_pos.shape[:-1], dtype=model_frame_occ_pos.dtype,
                            device=model_frame_occ_pos.device)
-        violation = -(interior_threshold + sdf_value)
+        violation = -interior_threshold + sdf_value
         loss[violating] = violation
-        loss = loss.sum(dim=-1)
         ctx.save_for_backward(violating, violation, sdf_value, sdf_grad)
         return loss
 
     @staticmethod
     def backward(ctx: Any, grad_outputs: Any) -> Any:
         # need to output the gradient of the loss w.r.t. all the inputs of forward
         dl_dsdf = None
@@ -139,41 +141,42 @@
         dl_dthreshold = None
         if ctx.needs_input_grad[1]:
             violating, violation, sdf_value, sdf_grad = ctx.saved_tensors
             # SDF grads point away from the surface; in this case we want to move the surface away from the occupied
             grads = torch.zeros(list(violating.shape) + [3], dtype=grad_outputs.dtype, device=grad_outputs.device)
             # free space point, so the surface needs to go in the opposite direction
             grads[violating] = violation.unsqueeze(-1) * sdf_grad
-            dl_dvoxels = grad_outputs[:, None, None] * -grads
+            dl_dvoxels = grad_outputs[:, :, None] * grads
 
         # gradients for the other inputs not implemented
         return dl_dsdf, dl_dvoxels, dl_dthreshold
 
 
 class KnownSDFLookupCost(torch.autograd.Function):
     @staticmethod
     def forward(ctx: Any, sdf: pv.ObjectFrameSDF, model_frame_positions: torch.tensor,
                 expected_sdf_values: torch.tensor) -> torch.tensor:
         # should be fast since they should be in cache
         sdf_value, sdf_grad = sdf(model_frame_positions)
         diff = sdf_value - expected_sdf_values
         # interior points will have sdf_value < 0
         ctx.save_for_backward(diff, sdf_grad)
-        return diff.abs().sum(dim=-1)
+        # return Batch x Points shape; caller should sum over points
+        return diff.abs()
 
     @staticmethod
     def backward(ctx: Any, grad_outputs: Any) -> Any:
         # need to output the gradient of the loss w.r.t. all the inputs of forward
         dl_dsdf = None
         dl_dx = None
         dl_dv = None
         if ctx.needs_input_grad[1]:
             diff, sdf_grad = ctx.saved_tensors
             grads = sdf_grad * diff.unsqueeze(-1)
-            dl_dx = grad_outputs[:, None, None] * grads
+            dl_dx = grad_outputs[:, :, None] * grads
 
         # gradients for the other inputs not implemented
         return dl_dsdf, dl_dx, dl_dv
 
 
 class KnownSDFVoxelDiffCost:
     @staticmethod
@@ -214,16 +217,17 @@
 
 class VolumetricCost(RegistrationCost):
     """Cost of transformed model pose intersecting with known freespace voxels"""
 
     def __init__(self, free_voxels: pv.Voxels, sdf_voxels: pv.Voxels,
                  obj_sdf: pv.ObjectFrameSDF,
                  surface_threshold=0.01,
+                 occ_voxels: pv.Voxels = None,
                  # cost scales
-                 scale=1, scale_known_freespace=1., scale_known_sdf=1.,
+                 scale=1, scale_known_freespace=1., scale_known_sdf=1., scale_known_occ=0,
                  device='cpu', dtype=torch.float,
                  # for some cost approximations for acceleration
                  query_voxel_grid: typing.Optional[pv.VoxelGrid] = None,
                  # for debugging only
                  vis=None, obj_factory=None,
                  debug=False, debug_known_sgd=False, debug_freespace=False):
         """
@@ -235,108 +239,156 @@
         """
 
         self.device = device
         self.dtype = dtype
 
         self.free_voxels = free_voxels
         self.sdf_voxels = sdf_voxels
+        self.occ_voxels = occ_voxels
 
         self.scale = scale
         self.scale_known_freespace = scale_known_freespace
         self.scale_known_sdf = scale_known_sdf
+        self.scale_known_occ = scale_known_occ
 
         # SDF gives us a volumetric representation of the target object
         self.sdf = obj_sdf
         self.surface_threshold = surface_threshold
 
+        # batch
+        self.B = None
+
+        # intermediate products for visualization purposes
+        self._last_call_info = {}
+        self._pts_interior = None
+        self._grad = None
+
+        self._pts_all = None
+        self.debug = debug
+        self.debug_known_sgd = debug_known_sgd
+        self.debug_freespace = debug_freespace
+
+        self.vis = vis
+        self.obj_factory = obj_factory
+
+        # model points for inverting the lookup of freespace cost
+        self.model_interior_points_orig = None
+        self.model_interior_normals_orig = None
+        self.model_interior_weights = None
+        self.model_all_points = None
+        self.model_all_weights = None
+        self.model_all_normals = None
+        self.model_interior_points = None
+        self.model_interior_normals = None
+        self.init_model_points(query_voxel_grid=query_voxel_grid)
+
+    @property
+    def last_call_info(self):
+        return self._last_call_info
+
+    def init_model_points(self, query_voxel_grid):
         # ---- for +, known free space points, we just have to care about interior points of the object
         # to facilitate comparison between volumes that are rotated, we sample points at the center of the object voxels
-        interior_threshold = -surface_threshold
+        interior_threshold = -self.surface_threshold
+        bb = self.sdf.surface_bounding_box(padding=0.1).cpu().numpy()
         if query_voxel_grid is None:
-            query_voxel_grid = pv.VoxelGrid(self.surface_threshold,
-                                            self.sdf.surface_bounding_box(padding=0.1).cpu().numpy(),
+            query_voxel_grid = pv.VoxelGrid(self.surface_threshold or 0.01,
+                                            bb,
                                             dtype=self.dtype, device=self.device)
 
         self.model_interior_points_orig = self.sdf.get_filtered_points(lambda voxel_sdf: voxel_sdf < interior_threshold,
                                                                        voxels=query_voxel_grid)
         if self.model_interior_points_orig.shape[0] == 0:
             raise RuntimeError("Something's wrong with the SDF since there are no interior points")
 
         self.model_interior_weights, self.model_interior_normals_orig = self.sdf(self.model_interior_points_orig)
         self.model_interior_weights *= -1
 
-        self.model_all_points = self.sdf.get_filtered_points(lambda voxel_sdf: voxel_sdf < surface_threshold,
+        self.model_all_points = self.sdf.get_filtered_points(lambda voxel_sdf: voxel_sdf < self.surface_threshold,
                                                              voxels=query_voxel_grid)
         self.model_all_weights, self.model_all_normals = self.sdf(self.model_all_points)
 
+        if self.model_interior_points_orig.shape[0] < 25:
+            logger.warning(
+                f"Only {self.model_interior_points_orig.shape[0]} interior points for the model; consider decreasing "
+                f"the surface threshold {self.surface_threshold} such as by decreasing resolution; "
+                f"the object bounding box is {bb}")
         if self.model_interior_points_orig.shape[0] == self.model_all_points.shape[0]:
             raise RuntimeError("The voxelgrid to query points is too small and only interior points have been "
                                "extracted. Resolve this by increasing the range the voxel grid is over")
-        # batch
-        self.B = None
 
-        # intermediate products for visualization purposes
-        self._last_call_info = {}
-        self._pts_interior = None
-        self._grad = None
-
-        self._pts_all = None
-        self.debug = debug
-        self.debug_known_sgd = debug_known_sgd
-        self.debug_freespace = debug_freespace
-
-        self.vis = vis
-        self.obj_factory = obj_factory
-
-    @property
-    def last_call_info(self):
-        return self._last_call_info
+    def build_model_points(self, R, T, s):
+        self.B = R.shape[0]
+        self.model_interior_points = self.model_interior_points_orig.repeat(self.B, 1, 1)
+        self.model_interior_normals = self.model_interior_normals_orig.repeat(self.B, 1, 1)
 
     def __call__(self, R, T, s, other_info=None):
         self._last_call_info = {}
         # assign batch and reuse for later for efficiency
         if self.B is None or self.B != R.shape[0]:
-            self.B = R.shape[0]
-            self.model_interior_points = self.model_interior_points_orig.repeat(self.B, 1, 1)
-            self.model_interior_normals = self.model_interior_normals_orig.repeat(self.B, 1, 1)
+            self.build_model_points(R, T, s)
 
         # voxels are in world frame
         # need points transformed into world frame
         # transform the points via the given similarity transformation parameters, then evaluate their occupancy
         # should transform the interior points from link frame to world frame
         self._transform_model_to_world_frame(R, T, s)
         # self.visualize(R, T, s)
 
-        loss = torch.zeros(self.B, device=self._pts_interior.device, dtype=self._pts_interior.dtype)
+        loss = torch.zeros(self.B, device=self.device, dtype=self.dtype)
 
         if self.scale_known_freespace != 0:
-            known_free_space_loss = FreeSpaceVoxelDiffCost.apply(self._pts_interior, self._grad,
-                                                                 self.model_interior_weights,
-                                                                 self.free_voxels)
-            loss += known_free_space_loss * self.scale_known_freespace
-            self._last_call_info['unscaled_known_free_space_loss'] = known_free_space_loss
+            loss += self._cost_freespace(R, T, s) * self.scale_known_freespace
+        if self.scale_known_occ != 0:
+            loss += self._cost_occ(R, T, s) * self.scale_known_occ
         if self.scale_known_sdf != 0:
-            known_sdf_voxel_centers, known_sdf_voxel_values = self.sdf_voxels.get_known_pos_and_values()
-            known_sdf_loss = KnownSDFVoxelDiffCost.apply(self._pts_all, self.model_all_weights,
-                                                         known_sdf_voxel_centers, known_sdf_voxel_values)
-            loss += known_sdf_loss * self.scale_known_sdf
-            self._last_call_info['unscaled_known_sdf_loss'] = known_sdf_loss
+            loss += self._cost_sdf(R, T, s) * self.scale_known_sdf
 
         return loss * self.scale
 
+    def _cost_freespace(self, R, T, s):
+        known_free_space_loss = FreeSpaceVoxelDiffCost.apply(self._pts_interior, self._grad,
+                                                             self.model_interior_weights,
+                                                             self.free_voxels)
+        self._last_call_info['unscaled_known_free_space_loss'] = known_free_space_loss
+        self._last_call_info["per_point_free_loss"] = None
+        return known_free_space_loss
+
+    def _cost_sdf(self, R, T, s):
+        known_sdf_voxel_centers, known_sdf_voxel_values = self.sdf_voxels.get_known_pos_and_values()
+        known_sdf_loss = KnownSDFVoxelDiffCost.apply(self._pts_all, self.model_all_weights,
+                                                     known_sdf_voxel_centers, known_sdf_voxel_values)
+        self._last_call_info['unscaled_known_sdf_loss'] = known_sdf_loss
+        return known_sdf_loss
+
+    def _cost_occ(self, R, T, s):
+        world_frame_occ_voxels, known_occ = self.occ_voxels.get_known_pos_and_values()
+        world_frame_occ_voxels = world_frame_occ_voxels[known_occ.view(-1) == 1]
+        model_frame_occ_voxels = self._transform_world_frame_points_to_model_frame(R, T, s,
+                                                                                   world_frame_occ_voxels)
+        known_occ_loss = OccupiedLookupCost.apply(self.sdf, model_frame_occ_voxels, self.surface_threshold)
+        known_occ_loss_per_tf = known_occ_loss.sum(dim=-1)
+        self._last_call_info["unscaled_known_occ_loss"] = known_occ_loss_per_tf
+        self._last_call_info["per_point_occ_loss"] = known_occ_loss
+        return known_occ_loss_per_tf
+
     def _transform_model_to_world_frame(self, R, T, s):
         Rt = R.transpose(-1, -2)
         tt = (-Rt @ T.reshape(-1, 3, 1)).squeeze(-1)
         self._pts_interior = apply_similarity_transform(self.model_interior_points, Rt, tt, s)
         self._pts_all = apply_similarity_transform(self.model_all_points, Rt, tt, s)
         if self.debug and self._pts_interior.requires_grad:
             self._pts_interior.retain_grad()
             self._pts_all.retain_grad()
         self._grad = apply_similarity_transform(self.model_interior_normals, Rt)
 
+    @staticmethod
+    def _transform_world_frame_points_to_model_frame(R, T, s, points):
+        return apply_similarity_transform(points, R, T, s)
+
     def visualize(self, R, T, s):
         if not self.debug:
             return
         if self.vis is not None:
             if self._pts_interior is None:
                 self._transform_model_to_world_frame(R, T, s)
             with torch.no_grad():
@@ -444,122 +496,50 @@
                         self.vis.clear_visualization_after("mingrad", i + 1)
                         self.vis.clear_visualization_after("intgrad", j + 1)
 
 
 class VolumetricDirectSDFCost(VolumetricCost):
     """Use SDF queries for the known SDF points instead of using cached grads"""
 
-    def __call__(self, R, T, s, other_info=None):
-        self._last_call_info = {}
-        if self.B is None or self.B != R.shape[0]:
-            self.B = R.shape[0]
-            self.model_interior_points = self.model_interior_points_orig.repeat(self.B, 1, 1)
-            self.model_interior_normals = self.model_interior_normals_orig.repeat(self.B, 1, 1)
-
-        # voxels are in world frame
-        self._transform_model_to_world_frame(R, T, s)
-
-        loss = torch.zeros(self.B, device=R.device, dtype=R.dtype)
-
-        if self.scale_known_freespace != 0:
-            known_free_space_loss = FreeSpaceVoxelDiffCost.apply(self._pts_interior, self._grad,
-                                                                 self.model_interior_weights,
-                                                                 self.free_voxels)
-            loss += known_free_space_loss * self.scale_known_freespace
-            self._last_call_info["unscaled_known_free_space_loss"] = known_free_space_loss
-        if self.scale_known_sdf != 0:
-            world_frame_known_sdf_voxels, known_sdf_values = self.sdf_voxels.get_known_pos_and_values()
-            known_sdf_model_frame = self._transform_world_frame_points_to_model_frame(R, T, s,
-                                                                                      world_frame_known_sdf_voxels)
-
-            known_sdf_loss = KnownSDFLookupCost.apply(self.sdf, known_sdf_model_frame, known_sdf_values)
-            loss += known_sdf_loss * self.scale_known_sdf
-            self._last_call_info["unscaled_known_sdf_loss"] = known_sdf_loss
-
-        return loss * self.scale
-
-    def _transform_world_frame_points_to_model_frame(self, R, T, s, points):
-        return apply_similarity_transform(points, R, T, s)
+    def _cost_sdf(self, R, T, s):
+        world_frame_known_sdf_voxels, known_sdf_values = self.sdf_voxels.get_known_pos_and_values()
+        known_sdf_model_frame = self._transform_world_frame_points_to_model_frame(R, T, s,
+                                                                                  world_frame_known_sdf_voxels)
+
+        known_sdf_loss = KnownSDFLookupCost.apply(self.sdf, known_sdf_model_frame, known_sdf_values)
+        known_sdf_loss_per_tf = known_sdf_loss.sum(dim=-1)
+        self._last_call_info["unscaled_known_sdf_loss"] = known_sdf_loss_per_tf
+        self._last_call_info["per_point_sdf_loss"] = known_sdf_loss
+        return known_sdf_loss_per_tf
 
 
-class VolumetricDoubleDirectCost(RegistrationCost):
+class VolumetricDoubleDirectCost(VolumetricDirectSDFCost):
     """Cost of transformed model pose intersecting with known freespace voxels
     (slower than the voxelized version above)"""
 
-    def __init__(self, free_voxels: pv.Voxels, sdf_voxels: pv.voxel.Voxels,
-                 obj_sdf: pv.ObjectFrameSDF,
-                 surface_threshold=0.01,
-                 # cost scales
-                 scale=1, scale_known_freespace=1., scale_known_sdf=1.,
-                 device='cpu', dtype=torch.float,
-                 # for debugging only
-                 vis=None, obj_factory=None,
-                 debug=False, debug_known_sgd=False, debug_freespace=False):
-        """
-        :param free_voxels: representation of freespace
-        :param sdf_voxels: voxels for which we know the exact SDF values for
-        :param obj_sdf: signed distance function of the target object in object frame
-        :param scale:
-        """
-
-        self.free_voxels = free_voxels
-        self.sdf_voxels = sdf_voxels
-
-        self.scale = scale
-        self.scale_known_freespace = scale_known_freespace
-        self.scale_known_sdf = scale_known_sdf
-
-        # SDF gives us a volumetric representation of the target object
-        self.sdf = obj_sdf
-        self.surface_threshold = surface_threshold
-
-        self.device = device
-        self.dtype = dtype
-
-        # batch
-        self.B = None
-
-        # intermediate products for visualization purposes
-        self.debug = debug
-        self.debug_known_sgd = debug_known_sgd
-        self.debug_freespace = debug_freespace
-
-        self.vis = vis
-        self.obj_factory = obj_factory
-
-    def __call__(self, R, T, s, other_info=None):
-        self._last_call_info = {}
-        # assign batch and reuse for later for efficiency
-        if self.B is None or self.B != R.shape[0]:
-            self.B = R.shape[0]
-
-        loss = torch.zeros(self.B, device=self.device, dtype=self.dtype)
+    def init_model_points(self, query_voxel_grid):
+        pass
 
-        # voxels are in world frame, translate them to model frame
-        if self.scale_known_freespace != 0:
-            world_frame_free_voxels, known_free = self.free_voxels.get_known_pos_and_values()
-            world_frame_free_voxels = world_frame_free_voxels[known_free.view(-1) == 1]
-            model_frame_free_voxels = self._transform_world_frame_points_to_model_frame(R, T, s,
-                                                                                        world_frame_free_voxels)
-            known_free_space_loss = FreeSpaceLookupCost.apply(self.sdf, model_frame_free_voxels, self.surface_threshold)
-            loss += known_free_space_loss * self.scale_known_freespace
-            self._last_call_info["unscaled_known_free_space_loss"] = known_free_space_loss
-        if self.scale_known_sdf != 0:
-            world_frame_known_sdf_voxels, known_sdf_values = self.sdf_voxels.get_known_pos_and_values()
-            known_sdf_model_frame = self._transform_world_frame_points_to_model_frame(R, T, s,
-                                                                                      world_frame_known_sdf_voxels)
-
-            known_sdf_loss = KnownSDFLookupCost.apply(self.sdf, known_sdf_model_frame, known_sdf_values)
-            loss += known_sdf_loss * self.scale_known_sdf
-            self._last_call_info["unscaled_known_sdf_loss"] = known_sdf_loss
+    def build_model_points(self, R, T, s):
+        self.B = R.shape[0]
 
-        return loss * self.scale
+    def _transform_model_to_world_frame(self, R, T, s):
+        # no model points needed
+        pass
 
-    def _transform_world_frame_points_to_model_frame(self, R, T, s, points):
-        return apply_similarity_transform(points, R, T, s)
+    def _cost_freespace(self, R, T, s):
+        world_frame_free_voxels, known_free = self.free_voxels.get_known_pos_and_values()
+        world_frame_free_voxels = world_frame_free_voxels[known_free.view(-1) == 1]
+        model_frame_free_voxels = self._transform_world_frame_points_to_model_frame(R, T, s,
+                                                                                    world_frame_free_voxels)
+        known_free_space_loss = FreeSpaceLookupCost.apply(self.sdf, model_frame_free_voxels, self.surface_threshold)
+        known_free_loss_per_tf = known_free_space_loss.sum(dim=-1)
+        self._last_call_info["unscaled_known_free_space_loss"] = known_free_loss_per_tf
+        self._last_call_info["per_point_free_loss"] = known_free_space_loss
+        return known_free_loss_per_tf
 
 
 class DiscreteNondifferentiableCost(RegistrationCost):
     """Flat high cost for any known free space point violations"""
 
     def __init__(self, free_voxels: pv.Voxels, sdf_voxels: pv.Voxels,
                  obj_sdf: pv.ObjectFrameSDF, scale=1,
```

### Comparing `chsel-0.1.3/src/chsel/initialization.py` & `chsel-0.2.0/src/chsel/initialization.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,22 +10,23 @@
 class InitMethod(enum.Enum):
     ORIGIN = 0
     CONTACT_CENTROID = 1
     RANDOM = 2
 
 
 def initialize_transform_estimates(B, freespace_ranges, init_method: InitMethod, contact_points,
-                                   device="cpu", dtype=torch.float):
+                                   device="cpu", dtype=torch.float, trans_noise=0.05):
     # translation is 0,0,0
     best_tsf_guess = random_upright_transforms(B, dtype, device)
     if init_method == InitMethod.ORIGIN:
         pass
     elif init_method == InitMethod.CONTACT_CENTROID:
         centroid = contact_points.mean(dim=0).to(device=device, dtype=dtype)
-        best_tsf_guess[:, :3, 3] = centroid
+        trans = np.random.uniform(np.ones(3) * -trans_noise, np.ones(3) * trans_noise, (B, 3))
+        best_tsf_guess[:, :3, 3] = centroid + torch.tensor(trans, device=device, dtype=dtype)
     elif init_method == InitMethod.RANDOM:
         trans = np.random.uniform(freespace_ranges[:, 0], freespace_ranges[:, 1], (B, 3))
         trans = torch.tensor(trans, device=device, dtype=dtype)
         best_tsf_guess[:, :3, 3] = trans
     else:
         raise RuntimeError(f"Unsupported initialization method: {init_method}")
     return best_tsf_guess
```

### Comparing `chsel-0.1.3/src/chsel/quality_diversity.py` & `chsel-0.2.0/src/chsel/quality_diversity.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,29 +3,33 @@
 import logging
 
 import cma
 import numpy as np
 
 import torch
 from arm_pytorch_utilities.tensor_utils import ensure_tensor
-from chsel.conversion import RT_to_continuous_representation, continuous_representation_to_RT
 
 from ribs.archives import GridArchive
 from ribs.emitters import EvolutionStrategyEmitter, GradientArborescenceEmitter
 from ribs.schedulers import Scheduler
 from chsel.costs import RegistrationCost
 from chsel.types import SimilarityTransform, ICPSolution
+from chsel.measure import PositionMeasure
 from chsel import registration_util
 
 logger = logging.getLogger(__name__)
 
 
+# try measure function on the rotation dimensions
+
+
 class QDOptimization:
     def __init__(self, registration_cost: RegistrationCost,
                  model_points_world_frame: torch.tensor,
+                 measure=None,
                  init_transform: Optional[SimilarityTransform] = None,
                  sigma=0.1,
                  num_emitters=5,
                  save_loss_plot=False,
                  savedir=registration_util.ROOT_DIR,
                  **kwargs):
         """
@@ -49,16 +53,20 @@
         self.sigma = sigma
         self.save_loss_plot = save_loss_plot
         self.savedir = savedir
 
         self.device = self.Xt.device
         self.dtype = self.Xt.dtype
 
+        self.measure = measure
+        if self.measure is None:
+            self.measure = PositionMeasure(2, dtype=self.dtype, device=self.device)
+
         Xt, R, T, s = registration_util.apply_init_transform(self.Xt, self.init_transform)
-        x = self.get_numpy_x(R, T)
+        x = self.measure.get_numpy_x(R, T)
         self.num_emitters = num_emitters
         self.scheduler = self.create_scheduler(x, **kwargs)
 
     def run(self):
         Xt, R, T, s = registration_util.apply_init_transform(self.Xt, self.init_transform)
 
         # initialize the transformation history
@@ -94,21 +102,14 @@
     def is_done(self):
         return False
 
     @abc.abstractmethod
     def get_all_elite_solutions(self):
         return None
 
-    @staticmethod
-    def get_numpy_x(R, T):
-        return RT_to_continuous_representation(R, T).cpu().numpy()
-
-    def get_torch_RT(self, x):
-        return continuous_representation_to_RT(x, self.device, self.dtype)
-
 
 class CMAES(QDOptimization):
     def create_scheduler(self, x, *args, **kwargs):
         x0 = x[0]
         options = {"popsize": self.B, "seed": np.random.randint(0, 10000), "tolfun": 1e-5, "tolfunhist": 1e-6}
         options.update(kwargs)
         es = cma.CMAEvolutionStrategy(x0=x0, sigma0=self.sigma, inopts=options)
@@ -116,108 +117,77 @@
 
     def is_done(self):
         return self.scheduler.stop()
 
     def step(self):
         solutions = self.scheduler.ask()
         # convert back to R, T, s
-        R, T = self.get_torch_RT(np.stack(solutions))
+        R, T = self.measure.get_torch_RT(np.stack(solutions))
         cost = self.registration_cost(R, T, None)
         self.scheduler.tell(solutions, cost.cpu().numpy())
         return cost
 
     def add_solutions(self, solutions):
         pass
 
     def get_all_elite_solutions(self):
         return None
 
     def process_final_results(self, s, losses):
         # convert ES back to R, T
         solutions = self.scheduler.ask()
-        R, T = self.get_torch_RT(np.stack(solutions))
+        R, T = self.measure.get_torch_RT(np.stack(solutions))
         rmse = self.registration_cost(R, T, s)
 
         if self.save_loss_plot:
             registration_util.plot_poke_losses(losses, savedir=self.savedir)
 
         return R, T, rmse
 
 
-# try measure function on the rotation dimensions
-def rot_measure(measure_dim, offset=0):
-    # ensure the measure is only over the rotation dimensions
-    assert measure_dim + offset <= 6
-
-    def fn(x):
-        return x[..., offset:measure_dim]
-
-    def grad(x):
-        grad = np.zeros((measure_dim, x.shape[-1]))
-        grad[:, offset:measure_dim] = np.eye(measure_dim)
-        grad = np.tile(grad, (x.shape[0], 1, 1))
-        return grad
-
-    return fn, grad
-
-
-def position_measure(measure_dim):
-    def fn(x):
-        return x[..., 6:6 + measure_dim]
-
-    def grad(x):
-        grad = np.zeros((measure_dim, x.shape[-1]))
-        grad[:, 6:6 + measure_dim] = np.eye(measure_dim)
-        grad = np.tile(grad, (x.shape[0], 1, 1))
-        return grad
-
-    return fn, grad
-
-
 class CMAME(QDOptimization):
     def __init__(self, *args, bins=20, iterations=100,
                  # require an explicit range
                  ranges=None,
                  outlier_ratio=5.0,  # reject solutions that are this many times worse than the best
+                 outlier_absolute_tolerance=1e-6,  # handle rmse = 0 by allowing for at least this much tolerance
                  qd_score_offset=-100,  # useful for tracking the archive QD score as monotonically increasing
-                 measure_dim=2,  # how many dimensions of translation to use, in the order of XYZ
-                 # custom measure function, overrides measure_dim
-                 measure_fn=None, measure_grad=None,
+                 measure=None,
                  **kwargs):
-        self.measure_dim = measure_dim
         if "sigma" not in kwargs:
             kwargs["sigma"] = 1.0
+        self.measure = measure
+        if self.measure is None:
+            self.measure = PositionMeasure(2)
+
         if isinstance(bins, (float, int)):
-            self.bins = [bins for _ in range(self.measure_dim)]
+            self.bins = [bins for _ in range(self.measure.measure_dim)]
         else:
-            assert len(bins) == self.measure_dim
+            assert len(bins) == self.measure.measure_dim
             self.bins = bins
         self.iterations = iterations
         self.ranges = ranges
         self.qd_score_offset = qd_score_offset
         self.outlier_ratio = outlier_ratio
+        self.outlier_absolute_tolerance = outlier_absolute_tolerance
 
         self.archive = None
         self.i = 0
         self.qd_scores = []
 
-        self._measure = measure_fn
-        self._measure_grad = measure_grad
-        if self._measure is None:
-            self._measure, self._measure_grad = position_measure(self.measure_dim)
-
-        super(CMAME, self).__init__(*args, **kwargs)
+        super(CMAME, self).__init__(*args, measure=self.measure, **kwargs)
 
     def _create_ranges(self):
         if self.ranges is None:
             raise RuntimeError("An explicit archive range must be specified")
 
     def create_scheduler(self, x, *args, **kwargs):
         self._create_ranges()
-        self.archive = GridArchive(solution_dim=x.shape[1], dims=self.bins, ranges=self.ranges[:self.measure_dim],
+        self.archive = GridArchive(solution_dim=x.shape[1], dims=self.bins,
+                                   ranges=self.ranges[:self.measure.measure_dim],
                                    seed=np.random.randint(0, 10000), qd_score_offset=self.qd_score_offset)
         emitters = [
             EvolutionStrategyEmitter(self.archive, x0=x[i], sigma0=self.sigma, batch_size=self.B,
                                      seed=np.random.randint(0, 10000)) for i in
             range(self.num_emitters)
         ]
         scheduler = Scheduler(self.archive, emitters)
@@ -227,62 +197,72 @@
         return self.i >= self.iterations
 
     def step(self):
         self.i += 1
         solutions = self.scheduler.ask()
         # evaluate the models and record the objective and behavior
         # note that objective is -cost
-        R, T = self.get_torch_RT(np.stack(solutions))
+        R, T = self.measure.get_torch_RT(np.stack(solutions))
         cost = self.registration_cost(R, T, None)
-        bcs = self._measure(solutions)
+        bcs = self.measure(solutions)
         self.scheduler.tell(-cost.cpu().numpy(), bcs)
         qd = self.archive.stats.norm_qd_score
         self.qd_scores.append(qd)
         logger.debug("step %d norm QD score: %f", self.i, qd)
         return cost
 
     def _add_solutions(self, solutions):
-        R, T = self.get_torch_RT(np.stack(solutions))
+        R, T = self.measure.get_torch_RT(np.stack(solutions))
         rmse = self.registration_cost(R, T, None)
-        self.archive.add(solutions, -rmse.cpu().numpy(), self._measure(solutions))
+        self.archive.add(solutions, -rmse.cpu().numpy(), self.measure(solutions))
 
     def add_solutions(self, solutions):
         if solutions is None:
             return
         assert isinstance(solutions, np.ndarray)
         SOLUTION_CHUNK = 300
         for i in range(0, solutions.shape[0], SOLUTION_CHUNK):
             self._add_solutions(solutions[i:i + SOLUTION_CHUNK])
 
     def get_all_elite_solutions(self):
-        df = self.archive.as_pandas()
-        solutions = df.solution_batch()
-        return solutions
+        return self.archive.data('solution')
 
     def process_final_results(self, s, losses):
-        df = self.archive.as_pandas()
-        objectives = df.objective_batch()
-        solutions = df.solution_batch()
+        objectives = self.archive.data('objective')
+        all_solutions = self.archive.data('solution')
 
         cost = -objectives
         # filter out all solutions that are more than outlier_ratio times worse than the best
         lowest_cost = np.min(cost)
-        inlier_mask = cost < lowest_cost * self.outlier_ratio
-        solutions = solutions[inlier_mask]
+        inlier_mask = cost < lowest_cost * self.outlier_ratio + self.outlier_absolute_tolerance
+        solutions = all_solutions[inlier_mask]
         cost = cost[inlier_mask]
+        # rather than min, resort to elites
+        if len(solutions) == 0:
+            cost = -objectives
+            elite_cost = np.quantile(cost, 0.01)
+            inlier_mask = cost < elite_cost * self.outlier_ratio
+            solutions = all_solutions[inlier_mask]
+            cost = cost[inlier_mask]
+        # if no elites, then resort to actual min
+        if len(solutions) == 0:
+            cost = -objectives
+            lowest_cost = np.min(cost)
+            solutions = all_solutions[cost == lowest_cost]
+            solutions = solutions.reshape(1, -1)
         if len(solutions) > self.B:
             order = np.argpartition(cost, self.B)
             solutions = solutions[order[:self.B]]
         # if there are fewer than B solutions, randomly sample the remaining ones from existing solutions
         elif len(solutions) < self.B:
             # sample from existing solutions with replacement by index
             resampled_indices = np.random.choice(np.arange(len(solutions)), self.B - len(solutions))
             solutions = np.concatenate([solutions, solutions[resampled_indices]], axis=0)
         # convert back to R, T
-        R, T = self.get_torch_RT(solutions)
+        R, T = self.measure.get_torch_RT(solutions)
         rmse = self.registration_cost(R, T, s)
 
         if self.save_loss_plot:
             registration_util.plot_poke_losses(losses, savedir=self.savedir)
             qd_scores = [torch.tensor(v).view(1) for v in self.qd_scores]
             registration_util.plot_poke_losses(qd_scores, savedir=self.savedir, loss_name='qd_score', logy=False,
                                                ylabel='norm qd score')
@@ -295,15 +275,15 @@
     def __init__(self, *args, lr=0.05, **kwargs):
         self.lr = lr
         super(CMAMEGA, self).__init__(*args, **kwargs)
 
     def create_scheduler(self, x, *args, **kwargs):
         self._create_ranges()
         self.archive = GridArchive(solution_dim=x.shape[1], dims=self.bins, seed=np.random.randint(0, 10000),
-                                   ranges=self.ranges[:self.measure_dim], qd_score_offset=self.qd_score_offset)
+                                   ranges=self.ranges[:self.measure.measure_dim], qd_score_offset=self.qd_score_offset)
         emitters = []
         # emitters += [
         #     EvolutionStrategyEmitter(self.archive, x0=x[i], sigma0=self.sigma, batch_size=self.B) for i in
         #     range(self.num_emitters)
         # ]
         # rb = 3
         # rot_bounds = np.array([[-rb, rb] for _ in range(6)])
@@ -314,29 +294,49 @@
                                         seed=np.random.randint(0, 10000)) for i in
             range(self.num_emitters)
         ]
         scheduler = Scheduler(self.archive, emitters)
         return scheduler
 
     def _f(self, x):
-        R, T = self.get_torch_RT(x)
+        R, T = self.measure.get_torch_RT(x)
         return self.registration_cost(R, T, None)
 
     def step(self):
         solutions = self.scheduler.ask_dqd()
-        bcs = self._measure(solutions)
+        bcs = self.measure(solutions)
         # evaluate the models and record the objective and behavior
         # note that objective is -cost
         # get objective gradient and also the behavior gradient
         x = ensure_tensor(self.device, self.dtype, solutions)
         x.requires_grad = True
         cost = self._f(x)
         cost.sum().backward()
         objective_grad = -(x.grad.cpu().numpy())
         objective = -cost.detach().cpu().numpy()
         objective_grad = objective_grad.reshape(x.shape[0], 1, -1)
-        measure_grad = self._measure_grad(x)
+        measure_grad = self.measure.grad(x)
 
         jacobian = np.concatenate((objective_grad, measure_grad), axis=1)
         self.scheduler.tell_dqd(objective, bcs, jacobian)
 
         return super(CMAMEGA, self).step()
+
+
+def initialize_qd_archive(T, rmse, measure_fn, outlier_ratio=5.0, outlier_absolute_tolerance=0.1, range_sigma=3,
+                          min_std=1e-4):
+    x = measure_fn.get_numpy_x(T[:, :3, :3], T[:, :3, 3])
+    measure = measure_fn(x)
+
+    # ensure the measure is 2D
+    measure = measure.reshape(-1, measure_fn.measure_dim)
+
+    # filter out any solution that is above outlier_ratio of the best solution found
+    keep = rmse < (rmse.min() * outlier_ratio + outlier_absolute_tolerance)
+    m = measure[keep.cpu()]
+    logger.info(f"keep {len(m)} solutions out of {len(measure)} for QD initialization with min rmse {rmse.min()}")
+
+    centroid, m_std = measure_fn.compute_moments(m)
+    m_std = np.maximum(m_std, min_std)
+
+    ranges = np.array((centroid - m_std * range_sigma, centroid + m_std * range_sigma)).T
+    return ranges.reshape(measure_fn.measure_dim, 2)
```

### Comparing `chsel-0.1.3/src/chsel/registration_util.py` & `chsel-0.2.0/src/chsel/registration_util.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 import os
 from typing import Optional
 
-import numpy as np
 import torch
 from matplotlib import pyplot as plt, cm as cm
 from ribs.visualize import grid_archive_heatmap
 from chsel.types import SimilarityTransform, ICPSolution
-from chsel.conversion import RT_to_continuous_representation
 import logging
 
 logger = logging.getLogger(__file__)
 
 poke_index = 0
 sgd_index = 0
 
@@ -131,36 +129,7 @@
         T[:, :3, :3] = res.RTs.R.transpose(-1, -2)
     else:
         T[:, :3, :3] = res.RTs.R
     T[:, :3, 3] = res.RTs.T
     return T
 
 
-def initialize_qd_archive(T, rmse, outlier_ratio=5.0, range_sigma=3, min_std=1e-4, measure_fn=None):
-    if measure_fn is None:
-        # by default the measure is the translation
-        measure = T[:, :3, 3]
-    else:
-        # measure_fn act on flattened pose representation
-        x = RT_to_continuous_representation(T[:, :3, :3], T[:, :3, 3])
-        measure = measure_fn(x)
-        # ensure the measure is 2D
-        if len(measure.shape) == 1:
-            measure = measure.reshape(1, -1)
-
-    # filter out any solution that is above outlier_ratio of the best solution found
-    keep = rmse < rmse.min() * outlier_ratio
-    m = measure[keep]
-    logger.info(f"keep {len(m)} solutions out of {len(measure)} for QD initialization")
-
-    centroid = m.mean(dim=-2).cpu().numpy()
-    if len(m) == 1:
-        m_std = min_std * np.ones_like(centroid)
-    else:
-        m_std = m.std(dim=-2).cpu().numpy()
-        m_std = np.maximum(m_std, min_std)
-
-    # extract translation measure
-    centroid = centroid
-    m_std = m_std
-    ranges = np.array((centroid - m_std * range_sigma, centroid + m_std * range_sigma)).T
-    return ranges
```

### Comparing `chsel-0.1.3/src/chsel/sgd.py` & `chsel-0.2.0/src/chsel/sgd.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 from typing import Optional
-
+import math
 import torch
 from chsel.costs import VolumetricCost
 from chsel.registration_util import plot_poke_losses, plot_sgd_losses
+from chsel.se2 import construct_plane_basis, xyz_to_uv, uv_to_xyz
 from chsel.types import SimilarityTransform, ICPSolution
+import pytorch_kinematics as pk
 from pytorch_kinematics import random_rotations, matrix_to_rotation_6d, rotation_6d_to_matrix
 
 import logging
+import typing
 
 logger = logging.getLogger(__file__)
 
 
 def volumetric_registration_sgd(
         volumetric_cost: VolumetricCost,
         batch=30,
@@ -164,22 +167,24 @@
             logger.info(f"ICP has not converged in {max_iterations} iterations.")
 
     return ICPSolution(converged, rmse, torch.empty(0), SimilarityTransform(R, T, s), t_history)
 
 
 def volumetric_points_alignment(
         volumetric_cost: VolumetricCost,
+        axis_of_rotation=None,
+        offset_along_axis=0,
         batch=30,
         estimate_scale: bool = False,
         R: torch.Tensor = None, T: torch.tensor = None, s: torch.tensor = None,
         iterations: int = 50,
         lr: float = 0.01,
         save_loss_plot=True,
         verbose=False
-) -> tuple[SimilarityTransform, torch.tensor]:
+) -> typing.Tuple[SimilarityTransform, torch.tensor]:
     """
     Finds a similarity transformation (rotation `R`, translation `T`
     and optionally scale `s`)  between two given sets of corresponding
     `d`-dimensional points `X` and `Y` such that:
 
     `s[i] X[i] R[i] + T[i] = Y[i]`,
 
@@ -196,14 +201,20 @@
 
     Returns:
         3-element named tuple `SimilarityTransform` containing
         - **R**: Batch of orthonormal matrices of shape `(minibatch, d, d)`.
         - **T**: Batch of translations of shape `(minibatch, d)`.
         - **s**: batch of scaling factors of shape `(minibatch, )`.
     """
+    if axis_of_rotation is not None:
+        return volumetric_points_alignment_2d(volumetric_cost, axis_of_rotation,
+                                              offset_along_axis=offset_along_axis, batch=batch,
+                                              estimate_scale=estimate_scale, R=R, T=T, s=s,
+                                              iterations=iterations, lr=lr, save_loss_plot=save_loss_plot,
+                                              verbose=verbose)
 
     device = volumetric_cost.device
     dtype = volumetric_cost.dtype
     # works for only 3D transforms
     dim = 3
 
     if R is None:
@@ -230,14 +241,92 @@
 
     losses = []
 
     for epoch in range(iterations):
         R, T = get_usable_transform_representation()
 
         total_loss = volumetric_cost(R, T, s)
+        total_loss.mean().backward()
+        losses.append(total_loss.detach())
+
+        # visualize gradients on the losses
+        volumetric_cost.visualize(R, T, s)
+
+        optimizer.step()
+        optimizer.zero_grad()
+
+    if save_loss_plot:
+        plot_sgd_losses(losses)
+
+    if verbose:
+        print(f"pose loss {total_loss.mean().item()}")
+    R, T = get_usable_transform_representation()
+    return SimilarityTransform(R.detach().clone(), T.detach().clone(),
+                               s.detach().clone()), total_loss.detach().clone()
+
+
+def volumetric_points_alignment_2d(
+        volumetric_cost: VolumetricCost,
+        axis_of_rotation: torch.tensor,
+        offset_along_axis=0,
+        batch=30,
+        estimate_scale: bool = False,
+        R: torch.Tensor = None, T: torch.tensor = None, s: torch.tensor = None,
+        iterations: int = 50,
+        lr: float = 0.01,
+        save_loss_plot=True,
+        verbose=False
+) -> typing.Tuple[SimilarityTransform, torch.tensor]:
+    """
+    Similar to above but for 2D transforms with a fixed axis of rotation
+    """
+    # ensure axis is normalized
+    axis_of_rotation = axis_of_rotation / torch.norm(axis_of_rotation)
+    origin = axis_of_rotation * offset_along_axis
+    axis_u, axis_v = construct_plane_basis(axis_of_rotation)
+
+    device = volumetric_cost.device
+    dtype = volumetric_cost.dtype
+    # works for only 3D transforms
+
+    if R is None:
+        theta = torch.rand(batch, dtype=dtype, device=device) * math.pi * 2
+        R = pk.axis_and_angle_to_matrix_33(axis_of_rotation, theta)
+        T = torch.randn((batch, 3), dtype=dtype, device=device)
+        s = torch.ones(batch, dtype=dtype, device=device)
+
+    # projection of rotation down to axis of rotation
+    axis_angle = pk.matrix_to_axis_angle(R)
+    # dot product against the given axis of rotation to get the angle
+    theta = axis_angle @ axis_of_rotation
+
+    # extract xy
+    # project them onto the SE(2) plane (offset along the axis)
+    uv = xyz_to_uv(T, origin, axis_of_rotation, axis_u, axis_v)
+
+    # set them up as parameters for training
+    theta.requires_grad = True
+    uv.requires_grad = True
+    if estimate_scale:
+        s.requires_grad = True
+
+    optimizer = torch.optim.Adam([theta, uv, s], lr=lr)
+
+    def get_usable_transform_representation():
+        nonlocal T
+        RR = pk.axis_and_angle_to_matrix_33(axis_of_rotation, theta)
+        T = uv_to_xyz(uv, origin, axis_u, axis_v)
+        return RR, T
+
+    losses = []
+
+    for epoch in range(iterations):
+        R, T = get_usable_transform_representation()
+
+        total_loss = volumetric_cost(R, T, s)
         total_loss.mean().backward()
         losses.append(total_loss.detach())
 
         # visualize gradients on the losses
         volumetric_cost.visualize(R, T, s)
 
         optimizer.step()
```

### Comparing `chsel-0.1.3/src/chsel/types.py` & `chsel-0.2.0/src/chsel/types.py`

 * *Files 18% similar despite different names*

```diff
@@ -17,14 +17,15 @@
     converged: bool
     rmse: Union[torch.Tensor, None]
     Xt: torch.Tensor
     RTs: SimilarityTransform
     t_history: List[SimilarityTransform]
 
 
-class SemanticsClass(enum.Enum):
-    FREE = 0
-    OCCUPIED = 1
+class SemanticsClass(enum.IntEnum):
+    SURFACE = 0
+    FREE = 1
+    OCCUPIED = 2
 
 
 # for known SDF value, it is the actual float value
 Semantics = Union[float, SemanticsClass]
```

### Comparing `chsel-0.1.3/src/chsel/wrapper.py` & `chsel-0.2.0/src/chsel/wrapper.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,206 +1,301 @@
-from typing import Sequence, Optional
+from typing import Sequence, Optional, Union
 
 import math
 import chsel
+import chsel.measure
+import chsel.quality_diversity
 import chsel.sgd
 import torch
 import numpy as np
 
 from chsel import costs
 from chsel import types
 from chsel import quality_diversity
 from chsel import registration_util
+from chsel.se2 import project_transform
 
 import pytorch_volumetric as pv
 import pytorch_kinematics as pk
 
 import logging
 
 logger = logging.getLogger(__file__)
 
 
+def ensure_tensor(device, dtype, *args):
+    tensors = tuple(
+        x.to(device=device, dtype=dtype) if torch.is_tensor(x) else
+        torch.tensor(x, device=device, dtype=dtype)
+        for x in args)
+    return tensors if len(tensors) > 1 else tensors[0]
+
+
 class CHSEL:
     def __init__(self,
                  obj_sdf: pv.ObjectFrameSDF,
                  positions: torch.tensor, semantics: Sequence[types.Semantics],
+                 resolution=None,
+                 known_sdf_values: Optional[torch.tensor] = None,
                  cost=costs.VolumetricDirectSDFCost,
                  free_voxels: Optional[pv.Voxels] = None,
                  occupied_voxels: Optional[pv.Voxels] = None,
                  known_sdf_voxels: Optional[pv.Voxels] = None,
-                 free_voxels_resolution=0.01,
+                 # parameters for SE2 registration
+                 axis_of_rotation=None,
+                 offset_along_axis=0,
+                 # for removing duplicate points
+                 free_voxels_resolution=None,
+                 occupied_voxels_resolution=None,
                  sgd_solution_outlier_rejection_ratio=5.0,
                  archive_range_sigma=3,
+                 archive_min_size=2e-4,
                  bins=40,
+                 do_qd=True,
                  qd_iterations=100,
                  qd_alg=quality_diversity.CMAMEGA,
-                 qd_measure_dim=2,
-                 qd_measure_fn=None,
-                 qd_measure_grad=None,
+                 qd_measure: Optional[chsel.measure.MeasureFunction] = None,
                  savedir=registration_util.ROOT_DIR,
                  debug=False,
                  qd_alg_kwargs=None,
                  **cost_kwargs):
         """
 
         :param obj_sdf: Object centered signed distance field (SDF)
         :param positions: World frame positions of the observed points
         :param semantics: Semantics of the observed points
+        :param resolution: Resolution in meters of the side-length of each voxel; this controls what points
+        are considered duplicates and removed when calling remove_duplicate_points(); if None is given, it will be
+        chosen such that there are at least 20 voxels per dimension of the object
+        :param known_sdf_values: Known SDF values of the observed points; if not specified, all known points will be
+        assumed to have SDF=0 (surface points)
         :param cost: Class that implements Eq. 6
         :param free_voxels: Explicit specification of free space voxels; if not specified they will be extracted
         from the given points that have the FREE semantics. If the observed points are derived from free voxels,
         it will save recreating them if these are specified directly.
         :param occupied_voxels: Similarly to the above
         :param known_sdf_voxels: Similarly to the above
-        :param free_voxels_resolution: Resolution in meters of the side-length of each voxel; this should scale with
-        the object's size; it is a good idea that at least 10 voxels span each dimension of the object
+        :param axis_of_rotation: If given, optimize over SE(2) instead of SE(3) by fixing the rotation around the given axis
+        :param offset_along_axis: If axis_of_rotation is given, the SE(2) optimization is over a plane defined by the
+        axis_of_rotation and offset from origin along the axis_of_rotation by this value
+        :param free_voxels_resolution: Resolution as above; this should scale with
+        the object's size; it is a good idea that at least 10 voxels span each dimension of the object. If set to None
+        by default, the duplicate resolution will be used
+        :param occupied_voxels_resolution: Similarly to the above
         :param sgd_solution_outlier_rejection_ratio: The ratio of CHSEL cost function to the best one found, above which
         to be considered an outlier and rejected. This is used to prevent the archive range being polluted with outliers
         :param archive_range_sigma: b_sigma the number of standard deviations to consider for the archive
+        :param archive_min_size: b_min the minimum size of the archive (range of the bin)
         :param bins: How many bins each dimension of the archive will have
+        :param do_qd: Whether to do quality diversity optimization
         :param qd_iterations: n_o number of quality diversity optimization iterations
         :param qd_alg: The quality diversity optimization algorithm to use
-        :param qd_measure_dim: The number of translation dimensions to use for the QD measure in the order of XYZ -
-        this is what is ensured diversity across. For example, if you use qd_measure_dim=2, only diversity of estimated
-        transforms across X and Y translation terms will be ensured. This may be useful if you have an upright prior
-        that the object lies on a plane normal to Z. Empirically, we found no significant difference in performance
-        between 2 and 3 dimensions.
-        :param qd_measure_fn: The function to use for the QD measure. If not specified, the position is used.
-        :param qd_measure_grad: The gradient of the QD measure function. If not specified, the one associated with
-        position is used.
+        :param qd_measure: The function to use for the QD measure. If not specified, the position is used.
         :param savedir: Directory to save loss plots
         :param debug:
         """
         self.obj_sdf = obj_sdf
         self.outlier_rejection_ratio = sgd_solution_outlier_rejection_ratio
+        self.resolution = resolution
+        if self.resolution is None:
+            bb = self.obj_sdf.surface_bounding_box()
+            r = bb[:, 1] - bb[:, 0]
+            self.resolution = (min(r) / 20).cpu().item()
+
+        self.axis_of_rotation = axis_of_rotation
+        self.offset_along_axis = offset_along_axis
 
         self.dtype = positions.dtype
         self.device = positions.device
 
         self.positions = positions
         # to allow batch indexing
-        semantics = np.asarray(semantics, dtype=object)
-        self.semantics = semantics
+        # store their numeric values rather than enum for better operations
+        self.semantics = ensure_tensor(self.device, torch.long, semantics)
 
         self.debug = debug
         self.archive_range_sigma = archive_range_sigma
+        self.archive_min_size = archive_min_size
         self.bins = bins
+        self.do_qd = do_qd
         self.qd_iterations = qd_iterations
         self.qd_alg = qd_alg
         self.savedir = savedir
         # extract indices
-        self._free = torch.tensor([s == chsel.SemanticsClass.FREE for s in semantics])
-        self._occupied = torch.tensor([s == chsel.SemanticsClass.OCCUPIED for s in semantics])
-        self._known = ~self._free & ~self._occupied
+        idx = CHSEL.get_separate_semantic_indices(self.semantics)
+        self._free = idx['free']
+        self._occupied = idx['occupied']
+        self._known = idx['known']
 
         # intermediate results for use outside for debugging
         self.res_init = None
         self.qd = None
         self.res_history = []
         self.res_init_history = []
 
-        self._qd_alg_kwargs = {"measure_dim": qd_measure_dim,
-                               "measure_fn": qd_measure_fn,
-                               "measure_grad": qd_measure_grad}
+        self._qd_alg_kwargs = {"measure": qd_measure, }
         if qd_alg_kwargs is not None:
             self._qd_alg_kwargs.update(qd_alg_kwargs)
 
         # extract the known free voxels from the given free points
         if free_voxels is None:
-            free_voxels = pv.ExpandingVoxelGrid(free_voxels_resolution, [(0, 0) for _ in range(3)], dtype=self.dtype,
+            free_voxels = pv.ExpandingVoxelGrid(free_voxels_resolution or self.resolution, [(0, 0) for _ in range(3)],
+                                                dtype=self.dtype,
                                                 device=self.device)
             free_voxels[positions[self._free]] = 1
-        # TODO extract the known occupied points (this has been unused in any experiments so far)
+        # extract the known occupied voxels from the given occupied points
+        if occupied_voxels is None:
+            occupied_voxels = pv.ExpandingVoxelGrid(occupied_voxels_resolution or self.resolution,
+                                                    [(0, 0) for _ in range(3)],
+                                                    dtype=self.dtype, device=self.device)
+            occupied_voxels[positions[self._occupied]] = 1
         # extract the known SDF points
         if known_sdf_voxels is None:
-            known_sdf_values = semantics[self._known].astype(float)
-            known_sdf_values = torch.tensor(known_sdf_values, dtype=self.dtype, device=self.device)
+            if known_sdf_values is None:
+                known_sdf_pts = positions[self._known]
+                known_sdf_values = torch.zeros(len(known_sdf_pts), dtype=self.dtype, device=self.device)
             known_sdf_voxels = pv.VoxelSet(positions[self._known], known_sdf_values)
 
         cost_options = {
             "scale_known_freespace": 20,
             "debug": self.debug,
-            "surface_threshold": free_voxels_resolution
+            "surface_threshold": self.resolution
         }
         cost_options.update(cost_kwargs)
         # construct the cost function
-        self.volumetric_cost = cost(free_voxels, known_sdf_voxels, self.obj_sdf, dtype=self.dtype, device=self.device,
+        self.volumetric_cost = cost(free_voxels, known_sdf_voxels, self.obj_sdf,
+                                    occ_voxels=occupied_voxels,
+                                    dtype=self.dtype, device=self.device,
                                     **cost_options)
 
-    def evaluate_homogeneous(self, H_world_to_link: torch.tensor, use_scale=False):
+    @staticmethod
+    def get_separate_semantic_indices(semantics):
+        free = semantics == chsel.SemanticsClass.FREE.value
+        occupied = semantics == chsel.SemanticsClass.OCCUPIED.value
+        known = ~free & ~occupied
+        return {'free': free, 'occupied': occupied, 'known': known}
+
+    def evaluate_homogeneous(self, H_world_to_link: Union[torch.tensor, pk.Transform3d], use_scale=False):
         """
         Evaluate the discrepency between the observed semantic point cloud and the given transforms (world to link)
         :return: the cost for each transform
         """
+        if not torch.is_tensor(H_world_to_link):
+            H_world_to_link = H_world_to_link.get_matrix()
         if use_scale:
             s = H_world_to_link[:, -1, -1]
         else:
             s = None
         return self.evaluate(H_world_to_link[:, :3, :3], H_world_to_link[:, :3, 3], s)
 
     def evaluate(self, R: torch.tensor, T: torch.tensor, s: torch.tensor = None):
         """
         Evaluate the discrepency between the observed semantic point cloud and the given transforms (world to link)
         :return: the cost for each transform
         """
         return self.volumetric_cost(R, T, s)
 
-    def update(self, positions, semantics):
+    def debug_last_cost_call(self):
+        return self.volumetric_cost.last_call_info
+
+    def update(self, positions: torch.tensor, semantics: torch.tensor, known_sdf_values=None):
         """
         Update the observed point cloud and semantics
         """
-        if len(positions) == 0:
+        if positions is None or len(positions) == 0:
             return
-        _free = torch.tensor([s == chsel.SemanticsClass.FREE for s in semantics])
-        _occupied = torch.tensor([s == chsel.SemanticsClass.OCCUPIED for s in semantics])
-        _known = ~_free & ~_occupied
+        idx = CHSEL.get_separate_semantic_indices(semantics)
+        _free = idx['free']
+        _occupied = idx['occupied']
+        _known = idx['known']
         self._free = torch.cat([self._free, _free])
         self._occupied = torch.cat([self._occupied, _occupied])
         self._known = torch.cat([self._known, _known])
         self.positions = torch.cat([self.positions, positions])
         self.volumetric_cost.free_voxels[positions[_free]] = 1
-        semantics = np.asarray(semantics, dtype=object)
-        self.semantics = np.concatenate([self.semantics, semantics])
+        self.semantics = torch.cat([self.semantics, semantics])
         if torch.any(_known):
             # special edge case for updating with only a single point, np interprets true as index 1
             if len(_known) == 1:
                 # if we directly use 0 as the index, the return is a scalar, so we need to use a slice
                 _known = slice(0, 1)
-            self.volumetric_cost.sdf_voxels[positions[_known]] = torch.tensor(semantics[_known].astype(float),
-                                                                              dtype=self.dtype,
-                                                                              device=self.device)
-
-    def undo_update(self, num_pts):
-        """
-        Undo the latest update
-        :param num_pts: number of points to remove, starting from the last added ones
-        """
-        free = self._free[-num_pts:]
-        pos = self.positions[-num_pts:]
-        # occupied = self._occupied[-num_pts:]
-        self.volumetric_cost.free_voxels[pos[free]] = 0
-
-        self._free = self._free[:-num_pts]
-        self._occupied = self._occupied[:-num_pts]
-        self._known = self._known[:-num_pts]
-        self.positions = self.positions[:-num_pts]
-
-        known_sdf_values = self.semantics[self._known].astype(float)
-        known_sdf_values = torch.tensor(known_sdf_values, dtype=self.dtype, device=self.device)
-        self.volumetric_cost.sdf_voxels = pv.VoxelSet(self.positions[self._known], known_sdf_values)
+            known_sdf_positions = positions[_known]
+            if known_sdf_values is None:
+                known_sdf_values = torch.zeros(len(known_sdf_positions), dtype=self.dtype, device=self.device)
+            self.volumetric_cost.sdf_voxels[known_sdf_positions] = known_sdf_values
+
+    def reset_free_points(self, still_free_points):
+        # don't touch the other semantics
+        untouched_semantics = self.semantics[~self._free]
+        positions = [self.positions[~self._free], still_free_points]
+        semantics = [untouched_semantics, torch.ones(len(still_free_points), dtype=torch.long,
+                                                     device=self.device) * chsel.SemanticsClass.FREE.value]
+
+        self.positions = torch.cat(positions)
+        self.semantics = torch.cat(semantics).reshape(-1)
+        self._build_semantic_indices()
+        self._sync_free_points()
+
+    def remove_duplicate_points(self, duplicate_distance=None, range_per_dim=None):
+        if duplicate_distance is None:
+            duplicate_distance = self.resolution
+
+        if range_per_dim is None:
+            range_per_dim = np.stack(
+                (self.positions.min(dim=0)[0].cpu().numpy(), self.positions.max(dim=0)[0].cpu().numpy())).T
+
+        all_pts = []
+        all_sem = []
+        for s in chsel.SemanticsClass:
+            # potentially different resolution per semantic class
+            if type(duplicate_distance) == dict:
+                resolution = duplicate_distance[s]
+            else:
+                resolution = duplicate_distance
+            idx = self.semantics == s.value
+            pts = self.positions[idx]
+            pts = pv.voxel_down_sample(pts, resolution, range_per_dim)
+            all_pts.append(pts)
+            all_sem.append(torch.ones(len(pts), dtype=torch.long, device=self.device) * s.value)
+        self.positions = torch.cat(all_pts)
+        self.semantics = torch.cat(all_sem).reshape(-1)
+        self._build_semantic_indices()
+
+        self._sync_sdf_points()
+        self._sync_free_points()
+
+    def _build_semantic_indices(self):
+        idx = CHSEL.get_separate_semantic_indices(self.semantics)
+        self._free = idx['free']
+        self._occupied = idx['occupied']
+        self._known = idx['known']
+
+    def _sync_free_points(self):
+        """Ensure the wrapper's free points are in sync with the volumetric cost function's free points"""
+        self.volumetric_cost.free_voxels = pv.ExpandingVoxelGrid(self.volumetric_cost.free_voxels.resolution,
+                                                                 [(0, 0) for _ in range(3)], dtype=self.dtype,
+                                                                 device=self.device)
+        self.volumetric_cost.free_voxels[self.positions[self._free]] = 1
+
+    def _sync_sdf_points(self):
+        known_sdf_positions = self.positions[self._known]
+        known_sdf_values = torch.zeros(len(known_sdf_positions), dtype=self.dtype, device=self.device)
+        self.volumetric_cost.sdf_voxels = pv.VoxelSet(known_sdf_positions, known_sdf_values)
 
     def register(self, iterations=1, initial_tsf=None, low_cost_transform_set=None, **kwargs):
         """
         Register the semantic point cloud to the given object SDF
         :param iterations: number of iterations to run
         :param initial_tsf: T_0 initial world to link transform to use for the optimization
         :param low_cost_transform_set: T_l low cost transform set such as from the previous iteration
         :param kwargs: arguments to pass to register_single
         :return: the registration result and all the archive solutions
         """
+        if initial_tsf is not None and isinstance(initial_tsf, pk.Transform3d):
+            initial_tsf = initial_tsf.get_matrix()
         res = None
         all_solutions = None
         self.res_history = []
         self.res_init_history = []
         for i in range(iterations):
             res, all_solutions = self.register_single(initial_tsf=initial_tsf,
                                                       low_cost_transform_set=low_cost_transform_set,
@@ -212,78 +307,110 @@
             # TODO auto select reinitialization policy based on RMSE distribution
             # reinitialize world_to_link around elites
             initial_tsf = chsel.reinitialize_transform_around_elites(world_to_link, res.rmse)
 
             low_cost_transform_set = all_solutions
         return res, all_solutions
 
-    def register_single(self, initial_tsf=None, low_cost_transform_set=None, batch=30, debug_func_after_sgd_init=None):
+    def enforce_transform_constraints(self, res):
+        if self.axis_of_rotation is not None:
+            R, T = project_transform(self.axis_of_rotation, self.offset_along_axis, res.RTs.R, res.RTs.T)
+            res = types.ICPSolution(res.converged, res.rmse, res.Xt, types.SimilarityTransform(R, T, res.RTs.s),
+                                    res.t_history)
+        return res
+
+    def register_single(self, initial_tsf=None, low_cost_transform_set=None, batch=30, debug_func_after_sgd_init=None,
+                        skip_qd=False):
         """
 
-        :param initial_tsf: T_0 initial transform to use for the optimization
+        :param initial_tsf: T_0 initial world to link transform to use for the optimization
         :param low_cost_transform_set: T_l low cost transform set such as from the previous iteration
         :param batch: number of transforms to estimate, only used if initial_tsf is not specified
         :param debug_func_after_sgd_init: debug function to call after the initial sgd optimization with the CHSEL
         object passed in
+        :param skip_qd: whether to skip the quality diversity optimization
         :return: the registration result (world to link transform matrix) and all the archive solutions
         """
+        if initial_tsf is not None and isinstance(initial_tsf, pk.Transform3d):
+            initial_tsf = initial_tsf.get_matrix()
+
         dim_pts = self.positions.shape[-1]
         known_pts_world_frame = self.positions[self._known]
         if initial_tsf is not None:
             batch = initial_tsf.shape[0]
 
         initial_tsf = init_random_transform_with_given_init(dim_pts, batch, self.dtype, self.device,
-                                                            initial_tsf=initial_tsf)
+                                                            initial_tsf=initial_tsf,
+                                                            axis_of_rotation=self.axis_of_rotation)
         initial_tsf = types.SimilarityTransform(initial_tsf[:, :3, :3],
                                                 initial_tsf[:, :3, 3],
                                                 torch.ones(batch, device=self.device, dtype=self.dtype))
 
         # feed it the result of SGD optimization
         self.res_init = chsel.sgd.volumetric_registration_sgd(self.volumetric_cost, batch=batch,
-                                                              init_transform=initial_tsf)
+                                                              init_transform=initial_tsf,
+                                                              axis_of_rotation=self.axis_of_rotation,
+                                                              offset_along_axis=self.offset_along_axis, )
+
+        if skip_qd or not self.do_qd:
+            self.res_init = self.enforce_transform_constraints(self.res_init)
+            return self.res_init, None
 
         # create range based on SGD results (where are good fits)
         # filter outliers out based on RMSE
         T = registration_util.solution_to_world_to_link_matrix(self.res_init)
-        archive_range = registration_util.initialize_qd_archive(T, self.res_init.rmse,
-                                                                outlier_ratio=self.outlier_rejection_ratio,
-                                                                range_sigma=self.archive_range_sigma,
-                                                                measure_fn=self._qd_alg_kwargs.get('measure_fn', None))
+        measure_fn = self._qd_alg_kwargs.get('measure', None)
+        if measure_fn is None:
+            if self.axis_of_rotation is None:
+                measure_fn = chsel.measure.PositionMeasure(2, device=self.device, dtype=self.dtype)
+            else:
+                measure_fn = chsel.measure.SE2AngleMeasure(axis_of_rotation=self.axis_of_rotation,
+                                                           offset_along_axis=self.offset_along_axis)
+        self._qd_alg_kwargs['measure'] = measure_fn
+        archive_range = chsel.quality_diversity.initialize_qd_archive(T, self.res_init.rmse, measure_fn,
+                                                                      outlier_ratio=self.outlier_rejection_ratio,
+                                                                      range_sigma=self.archive_range_sigma,
+                                                                      min_std=self.archive_min_size * 0.5)
         logger.info("QD position bins %s %s", self.bins, archive_range)
 
         if debug_func_after_sgd_init is not None:
             debug_func_after_sgd_init(self)
 
         # run QD
         self.qd = self.qd_alg(self.volumetric_cost, known_pts_world_frame.repeat(batch, 1, 1),
                               init_transform=initial_tsf,
                               outlier_ratio=self.outlier_rejection_ratio,
                               iterations=self.qd_iterations, num_emitters=1, bins=self.bins,
                               ranges=archive_range, savedir=self.savedir, **self._qd_alg_kwargs)
 
         # \hat{T}_0
-        x = self.qd.get_numpy_x(self.res_init.RTs.R, self.res_init.RTs.T)
+        x = self.qd.measure.get_numpy_x(self.res_init.RTs.R, self.res_init.RTs.T)
         self.qd.add_solutions(x)
         # \hat{T}_l (such as from the previous iteration's get_all_elite_solutions())
         self.qd.add_solutions(low_cost_transform_set)
 
         res = self.qd.run()
+        res = self.enforce_transform_constraints(res)
 
         return res, self.qd.get_all_elite_solutions()
 
 
-def init_random_transform_with_given_init(m, batch, dtype, device, initial_tsf=None):
+def init_random_transform_with_given_init(m, batch, dtype, device, initial_tsf=None, axis_of_rotation=None):
     # apply some random initial poses
-    if m > 2:
+    if m > 2 and axis_of_rotation is None:
         R = pk.random_rotations(batch, dtype=dtype, device=device)
     else:
         theta = torch.rand(batch, dtype=dtype, device=device) * math.pi * 2
-        Rtop = torch.cat([torch.cos(theta).view(-1, 1), -torch.sin(theta).view(-1, 1)], dim=1)
-        Rbot = torch.cat([torch.sin(theta).view(-1, 1), torch.cos(theta).view(-1, 1)], dim=1)
-        R = torch.cat((Rtop.unsqueeze(-1), Rbot.unsqueeze(-1)), dim=-1)
+        if axis_of_rotation is not None:
+            # rotate around the given axis
+            R = pk.axis_and_angle_to_matrix_33(axis_of_rotation, theta)
+        else:
+            Rtop = torch.cat([torch.cos(theta).view(-1, 1), -torch.sin(theta).view(-1, 1)], dim=1)
+            Rbot = torch.cat([torch.sin(theta).view(-1, 1), torch.cos(theta).view(-1, 1)], dim=1)
+            R = torch.cat((Rtop.unsqueeze(-1), Rbot.unsqueeze(-1)), dim=-1)
 
     init_pose = torch.eye(m + 1, dtype=dtype, device=device).repeat(batch, 1, 1)
     init_pose[:, :m, :m] = R[:, :m, :m]
     if initial_tsf is not None:
         # check if it's given as a batch
         if len(initial_tsf.shape) == 3:
             init_pose = initial_tsf.clone()
```

### Comparing `chsel-0.1.3/src/chsel.egg-info/PKG-INFO` & `chsel-0.2.0/src/chsel.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chsel
-Version: 0.1.3
+Version: 0.2.0
 Summary: Constrained pose Hypothesis Set Elimination official code for pose estimation
 Author-email: Sheng Zhong <zhsh@umich.edu>
 Maintainer-email: Sheng Zhong <zhsh@umich.edu>
 License: Copyright (c) 2023 University of Michigan ARM Lab
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the "Software"), to deal in
@@ -30,18 +30,28 @@
 Project-URL: Source, https://github.com/UM-ARM-Lab/chsel
 Keywords: robotics,pose estimation,registration,pytorch
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Python: >=3.6
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
-Provides-Extra: test
 License-File: LICENSE.txt
+Requires-Dist: cma
+Requires-Dist: torch
+Requires-Dist: numpy
+Requires-Dist: matplotlib
+Requires-Dist: arm-pytorch-utilities
+Requires-Dist: pytorch-kinematics
+Requires-Dist: pytorch-volumetric
+Requires-Dist: cma
+Requires-Dist: ribs[all]
+Provides-Extra: test
+Requires-Dist: pytest; extra == "test"
 
 ## CHSEL: Producing Diverse Plausible Pose Estimates from Contact and Free Space Data
 
 ![combined demo](https://i.imgur.com/T4DnKDu.gif)
 
 Demo CHSEL results on drill with sparse contact data (top) and mug with dense vision data (bottom).
 
@@ -67,14 +77,39 @@
   year={2023}
 }
 ```
 
 To reproduce the results from the paper, see the 
 [experiments repository](https://github.com/UM-ARM-Lab/chsel_experiments).
 
+## Intuition
+### Cost
+* enforce an object's signed distance field (SDF) consistency against point clouds augmented with volumetric semantics
+    * whether a point is in free space, inside the object, or has a known SDF value 
+* two of those semantics classes encodes uncertainty about the observed point's SDF
+    * for example free space just means we know the point has SDF > 0, but makes no claim about its actual value
+    * in many observation scenarios, we do not know the observed' point's actual SDF value
+* compared to related methods like SDF2SDF that match an SDF against another SDF, this avoids bias
+
+### Optimization
+At a high level, our method can be summarized as:
+1. start with an initial set of transforms that ideally covers all local minima
+   * for every local minima, there exists a transform in the initial set that is in its attraction basin in terms of the local cost landscape
+3. find the bounds of the local minima landscape
+    * usually much smaller than the whole search space
+    * do this by performing gradient descent independently on each initial transform with our given cost
+4. consider search in a dimensionality reduced feature space
+    * translational component of the transform such that we consider the best rotation for each translation
+6. find good local minima with a fine-tuning search with the search space reduced to the local minima bounds that we found to afford higher resolution
+    * instead of finding the best local minima, we want to evaluate all local minima, and we do this with Quality Diversity optimization on the feature space
+    * we maintain an archive, a grid in feature space, each cell of which holds the best solution given that archive (so the grid is in translation space, and each cell holds a full transform)
+    * we populate this archive over the course of QD optimization, which evolutionarily combines the top solutions
+7. we return the transforms from the best scoring cells, as many as requested
+    * usually same number as in the input transform set
+
 ## Usage
 CHSEL registers an observed semantic point cloud against a target object's signed distance field (SDF).
 It is agnostic to how the semantic point cloud is obtained, which can come from cameras and tactile sensors for example.
 
 Example code is given in `tests/test_wrapper.py`.
 
 First you need an object frame SDF which you can generate from its 3D mesh
@@ -325,7 +360,35 @@
 # feed all solutions from the previous iteration
 # assuming the object hasn't moved, use the output of the previous iteration as the initial estimate
 # this res is from the last iteration of the previous registration
 world_to_link = chsel.solution_to_world_to_link_matrix(res)
 res, all_solutions = registration.register(iterations=5, batch=B, initial_tsf=world_to_link,
                                            low_cost_transform_set=all_solutions)
 ```
+
+### SE(2) Constraint
+If you know the object lies on a table top for example, you can constrain the optimization to be over
+SE(2) instead of SE(3). You do this by specifying the plane via the axis of rotation (normal) and a
+scalar offset:
+```python
+# table top assumed to face positive z
+normal = torch.tensor([0, 0, 1])
+offset = torch.tensor([0, 0, 0])
+registration = chsel.CHSEL(sdf, positions, semantics, axis_of_rotation=normal, offset_along_normal=offset)
+```
+
+### Measures
+QD optimization works by binning over the measure space. This is how diversity is enforced.
+You can specify the measure space by providing a `chsel.measure.MeasureFunction` object.
+Note that this also defines what space the QD optimization is performed in. (such as a 9 dimensional continuous 
+representation of SE(3) transforms, or a 3 dimensional space for SE(2) transforms).
+
+For example, if you are on a tabletop and know the object's position quite well and want diversity in yaw:
+
+```python
+import chsel
+
+normal = torch.tensor([0, 0, 1])
+offset = torch.tensor([0, 0, 0])
+measure = chsel.SE2AngleMeasure(axis_of_rotation=normal, offset_along_normal=offset)
+registration = chsel.CHSEL(sdf, positions, semantics, axis_of_rotation=normal, offset_along_normal=offset)
+```
```

### Comparing `chsel-0.1.3/tests/test_wrapper.py` & `chsel-0.2.0/tests/test_wrapper.py`

 * *Files 6% similar despite different names*

```diff
@@ -101,32 +101,33 @@
         pc_occupied.points = o3d.utility.Vector3dVector(pts_occupied.cpu().numpy())
         pc_occupied.paint_uniform_color([0, 0.706, 0])
 
         pc_sdf = o3d.geometry.PointCloud()
         pc_sdf.points = o3d.utility.Vector3dVector(pts_sdf.cpu().numpy())
         pc_sdf.paint_uniform_color([0, 0.706, 1])
 
-        print(f"visualize object mesh, free space points (orange), and known SDF points (blue) (press Q or the close window button to move on)")
+        print(
+            f"visualize object mesh, free space points (orange), and known SDF points (blue) (press Q or the close window button to move on)")
         draw_geometries_one_rotation([obj._mesh, pc_free, pc_occupied, pc_sdf])
 
-
     gt_tf = pk.Transform3d(pos=torch.randn(3, device=d), rot=pk.random_rotation(device=d), device=d)
     positions = gt_tf.transform_points(positions_obj_frame)
 
     # visualize the transformed mesh and points
     if visualize:
         link_to_world_gt = gt_tf.get_matrix()[0]
         tf_mesh = copy.deepcopy(obj._mesh).transform(link_to_world_gt.cpu().numpy())
         pts_free = positions[_free]
         pts_sdf = positions[_known]
 
         # only plotting the transformed known SDF points for clarity
         pc_free.points = o3d.utility.Vector3dVector(pts_free.cpu())
         pc_sdf.points = o3d.utility.Vector3dVector(pts_sdf.cpu())
-        print(f"visualize the transformed object mesh, free space points, and known SDF points (press Q or the close window button to move on)")
+        print(
+            f"visualize the transformed object mesh, free space points, and known SDF points (press Q or the close window button to move on)")
         draw_geometries_one_rotation([tf_mesh, pc_free, pc_sdf])
 
     def visualize_transforms(link_to_world):
         # visualize the transformed mesh and points
         if visualize:
             # est_tf = pk.Transform3d(matrix=world_to_link.inverse())
             geo = [tf_mesh, pc_free, pc_sdf]
@@ -134,15 +135,30 @@
                 tfd_mesh = copy.deepcopy(obj._mesh).transform(link_to_world[i].cpu().numpy())
                 # paint tfd_mesh a color corresponding to the index in the batch
                 tfd_mesh.paint_uniform_color([i / (B * 2), 0, 1 - i / (B * 2)])
                 geo.append(tfd_mesh)
 
             draw_geometries_one_rotation(geo)
 
-    registration = chsel.CHSEL(sdf, positions, semantics, qd_iterations=100, free_voxels_resolution=0.005)
+    registration = chsel.CHSEL(sdf, positions, semantics, qd_iterations=100, do_qd=True)
+    if visualize:
+        # visualize the model points (in model frame)
+        interior_pts = registration.volumetric_cost.model_interior_points_orig
+        if interior_pts is not None:
+            pc_interior = o3d.geometry.PointCloud()
+            pc_interior.points = o3d.utility.Vector3dVector(interior_pts.cpu().numpy())
+            pc_interior.paint_uniform_color([0, 0, 1])
+
+            all_pts = registration.volumetric_cost.model_all_points
+            pc_all = o3d.geometry.PointCloud()
+            pc_all.points = o3d.utility.Vector3dVector(all_pts.cpu().numpy())
+            pc_all.paint_uniform_color([0, 1, 0])
+
+            draw_geometries_one_rotation([pc_all, pc_interior])
+
     # with no initial transform guess (starts guesses with random rotations at the origin)
     # we want a set of 30 transforms
     random_init_tsf = pk.Transform3d(pos=torch.randn((B, 3), device=d), rot=pk.random_rotations(B, device=d), device=d)
     random_init_tsf = random_init_tsf.get_matrix()
 
     # try to use the ground truth transform as the initial guess
     # gt_init = chsel.reinitialize_transform_estimates(B, gt_tf.inverse().get_matrix()[0])
@@ -155,19 +171,24 @@
         for i in range(iterations):
             print(f"iteration {i}")
             start = timer()
             # assuming the object hasn't moved, use the output of the previous iteration as the initial estimate
             res, all_solutions = registration.register(initial_tsf=world_to_link, batch=B,
                                                        low_cost_transform_set=all_solutions)
             print(f"registration took {timer() - start} seconds")
+            # print the RMSE for each cost type
 
             world_to_link = chsel.solution_to_world_to_link_matrix(res)
             link_to_world = world_to_link.inverse()
             # print sorted rmse
             print(torch.sort(res.rmse))
+            fl = registration.debug_last_cost_call().get('unscaled_known_free_space_loss')
+            sl = registration.debug_last_cost_call().get('unscaled_known_sdf_loss')
+            ol = registration.debug_last_cost_call().get('unscaled_known_occ_loss')
+            print(f"free space loss {fl} \nsdf loss {sl} \nocc loss {ol}")
             visualize_transforms(link_to_world)
 
             # reinitialize world_to_link around elites
             world_to_link = chsel.reinitialize_transform_around_elites(world_to_link, res.rmse)
     else:
         res, all_solutions = registration.register(iterations=iterations, batch=B, initial_tsf=random_init_tsf)
         print("Showing each iteration of the registration result (press Q or the close window button to move on)")
@@ -217,27 +238,26 @@
                                                   torch.ones(B, device=d, dtype=model_points_register.dtype))
     except ImportError:
         print("Install pytorch3d to run ICP")
 
     # manually do single step registrations (iterations=1 essentially)
 
 
-
-def test_chsel_on_drill(rng_seed=3):
+def test_chsel_on_drill(rng_seed=1):
     seed(rng_seed)
     # supposing we have an object mesh (most formats supported) - from https://github.com/eleramp/pybullet-object-models
     obj = pv.MeshObjectFactory(os.path.join(TEST_DIR, "YcbPowerDrill/textured_simple_reoriented.obj"))
     sdf = pv.MeshSDF(obj)
 
     # get some points in a grid in the object frame (can get points through other means)
     # this is only around one part of the object to simulate the local nature of contacts
     query_range = np.array([
-        [0.04, 0.15],
-        [0.04, 0.15],
-        [0.1, 0.25],
+        [0.01, 0.15],
+        [0.01, 0.15],
+        [0.05, 0.2],
     ])
 
     coords, pts = pv.get_coordinates_and_points_in_grid(0.005, query_range, device=d)
 
     # randomly permute points so they are not in order
     pts = pts[torch.randperm(len(pts))]
 
@@ -245,15 +265,15 @@
     # assuming we only observe surface points, set thresholds for known free and known occupied
     # note that this is the most common case, but you can know non-zero (non-surface) SDF values
     known_free = sdf_val > 0.005
     known_occupied = sdf_val < -0.005
     known_sdf = ~known_free & ~known_occupied
 
     # randomly downsample (we randomly permutated before) to simulate getting partial observations
-    N = 100
+    N = 200
 
     # group and stack the points together
     # note that it will still work even if you don't have all 3 or even 2 classes
     # for example with only known surface points, it degenerates to a form of ICP
     # we also don't need balanced data from each class
     pts_free = pts[known_free][:N]
     pts_occupied = pts[known_occupied][:N]
@@ -266,11 +286,12 @@
     positions = torch.cat((pts_free, pts_occupied, pts_sdf))
     semantics = sem_free + sem_occupied + sem_sdf.tolist()
     test_chsel_on_obj(obj, sdf, positions, semantics)
 
 
 if __name__ == "__main__":
     rng_seed = int(sys.argv[1]) if len(sys.argv) > 1 else 3
-    print(f"Using random seed {rng_seed}; try running with different seeds to see different results with\npython tests/test_wrapper.py <seed>")
+    print(
+        f"Using random seed {rng_seed}; try running with different seeds to see different results with\npython tests/test_wrapper.py <seed>")
     if not torch.cuda.is_available():
         print("Warning: CUDA not available, running on CPU which may be much slower")
     test_chsel_on_drill(rng_seed)
```

