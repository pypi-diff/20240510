# Comparing `tmp/openmc_source_plotter-0.7.0.tar.gz` & `tmp/openmc_source_plotter-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openmc_source_plotter-0.7.0.tar", last modified: Fri Mar  8 14:48:09 2024, max compression
+gzip compressed data, was "openmc_source_plotter-0.7.1.tar", last modified: Fri May 10 21:36:57 2024, max compression
```

## Comparing `openmc_source_plotter-0.7.0.tar` & `openmc_source_plotter-0.7.1.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 14:48:09.169975 openmc_source_plotter-0.7.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 14:48:09.165975 openmc_source_plotter-0.7.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 14:48:09.165975 openmc_source_plotter-0.7.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      606 2024-03-08 14:47:58.000000 openmc_source_plotter-0.7.0/.github/workflows/black.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-03-08 14:47:58.000000 openmc_source_plotter-0.7.0/.github/workflows/ci_with_install.yml
--rw-r--r--   0 runner    (1001) docker     (127)      544 2024-03-08 14:47:58.000000 openmc_source_plotter-0.7.0/.github/workflows/lint.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-03-08 14:47:58.000000 openmc_source_plotter-0.7.0/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1929 2024-03-08 14:47:58.000000 openmc_source_plotter-0.7.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-03-08 14:47:58.000000 openmc_source_plotter-0.7.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6511 2024-03-08 14:48:09.169975 openmc_source_plotter-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4346 2024-03-08 14:47:58.000000 openmc_source_plotter-0.7.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-03-08 14:47:58.000000 openmc_source_plotter-0.7.0/environment.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 14:48:09.165975 openmc_source_plotter-0.7.0/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-03-08 14:47:58.000000 openmc_source_plotter-0.7.0/examples/example_gamma_spec_plot.py
--rw-r--r--   0 runner    (1001) docker     (127)      592 2024-03-08 14:47:58.000000 openmc_source_plotter-0.7.0/examples/example_get_particle_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      949 2024-03-08 14:47:58.000000 openmc_source_plotter-0.7.0/examples/example_plot_plasma_source_position.py
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-03-08 14:47:58.000000 openmc_source_plotter-0.7.0/examples/example_plot_source_direction.py
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-03-08 14:47:58.000000 openmc_source_plotter-0.7.0/examples/example_plot_source_energy.py
--rw-r--r--   0 runner    (1001) docker     (127)      774 2024-03-08 14:47:58.000000 openmc_source_plotter-0.7.0/examples/example_plot_source_position.py
--rw-r--r--   0 runner    (1001) docker     (127)      691 2024-03-08 14:47:58.000000 openmc_source_plotter-0.7.0/examples/example_plot_two_source_energies.py
--rw-r--r--   0 runner    (1001) docker     (127)    24631 2024-03-08 14:47:58.000000 openmc_source_plotter-0.7.0/examples/gamma_spec.png
--rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-03-08 14:47:58.000000 openmc_source_plotter-0.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-08 14:48:09.169975 openmc_source_plotter-0.7.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 14:48:09.165975 openmc_source_plotter-0.7.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 14:48:09.169975 openmc_source_plotter-0.7.0/src/openmc_source_plotter/
--rw-r--r--   0 runner    (1001) docker     (127)      527 2024-03-08 14:47:58.000000 openmc_source_plotter-0.7.0/src/openmc_source_plotter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-03-08 14:48:09.000000 openmc_source_plotter-0.7.0/src/openmc_source_plotter/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     8631 2024-03-08 14:47:58.000000 openmc_source_plotter-0.7.0/src/openmc_source_plotter/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     2655 2024-03-08 14:47:58.000000 openmc_source_plotter-0.7.0/src/openmc_source_plotter/material.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 14:48:09.169975 openmc_source_plotter-0.7.0/src/openmc_source_plotter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6511 2024-03-08 14:48:09.000000 openmc_source_plotter-0.7.0/src/openmc_source_plotter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-03-08 14:48:09.000000 openmc_source_plotter-0.7.0/src/openmc_source_plotter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-08 14:48:09.000000 openmc_source_plotter-0.7.0/src/openmc_source_plotter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-03-08 14:48:09.000000 openmc_source_plotter-0.7.0/src/openmc_source_plotter.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-03-08 14:48:09.000000 openmc_source_plotter-0.7.0/src/openmc_source_plotter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-08 14:48:09.000000 openmc_source_plotter-0.7.0/src/openmc_source_plotter.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 14:48:09.169975 openmc_source_plotter-0.7.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2689 2024-03-08 14:47:58.000000 openmc_source_plotter-0.7.0/tests/test_core_with_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2512 2024-03-08 14:47:58.000000 openmc_source_plotter-0.7.0/tests/test_core_with_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     2842 2024-03-08 14:47:58.000000 openmc_source_plotter-0.7.0/tests/test_core_with_source.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-08 14:47:58.000000 openmc_source_plotter-0.7.0/tests/todo.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 21:36:57.172985 openmc_source_plotter-0.7.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 21:36:57.164986 openmc_source_plotter-0.7.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 21:36:57.164986 openmc_source_plotter-0.7.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2024-05-10 21:36:46.000000 openmc_source_plotter-0.7.1/.github/workflows/black.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-05-10 21:36:46.000000 openmc_source_plotter-0.7.1/.github/workflows/ci_with_install.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      544 2024-05-10 21:36:46.000000 openmc_source_plotter-0.7.1/.github/workflows/lint.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-05-10 21:36:46.000000 openmc_source_plotter-0.7.1/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1929 2024-05-10 21:36:46.000000 openmc_source_plotter-0.7.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-10 21:36:46.000000 openmc_source_plotter-0.7.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6511 2024-05-10 21:36:57.172985 openmc_source_plotter-0.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4346 2024-05-10 21:36:46.000000 openmc_source_plotter-0.7.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-10 21:36:46.000000 openmc_source_plotter-0.7.1/environment.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 21:36:57.168985 openmc_source_plotter-0.7.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-05-10 21:36:46.000000 openmc_source_plotter-0.7.1/examples/example_gamma_spec_plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-05-10 21:36:46.000000 openmc_source_plotter-0.7.1/examples/example_get_particle_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      949 2024-05-10 21:36:46.000000 openmc_source_plotter-0.7.1/examples/example_plot_plasma_source_position.py
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-10 21:36:46.000000 openmc_source_plotter-0.7.1/examples/example_plot_source_direction.py
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-10 21:36:46.000000 openmc_source_plotter-0.7.1/examples/example_plot_source_energy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      774 2024-05-10 21:36:46.000000 openmc_source_plotter-0.7.1/examples/example_plot_source_position.py
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-05-10 21:36:46.000000 openmc_source_plotter-0.7.1/examples/example_plot_two_source_energies.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24631 2024-05-10 21:36:46.000000 openmc_source_plotter-0.7.1/examples/gamma_spec.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-05-10 21:36:46.000000 openmc_source_plotter-0.7.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 21:36:57.172985 openmc_source_plotter-0.7.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 21:36:57.164986 openmc_source_plotter-0.7.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 21:36:57.168985 openmc_source_plotter-0.7.1/src/openmc_source_plotter/
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-05-10 21:36:47.000000 openmc_source_plotter-0.7.1/src/openmc_source_plotter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-10 21:36:57.000000 openmc_source_plotter-0.7.1/src/openmc_source_plotter/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8631 2024-05-10 21:36:47.000000 openmc_source_plotter-0.7.1/src/openmc_source_plotter/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2952 2024-05-10 21:36:47.000000 openmc_source_plotter-0.7.1/src/openmc_source_plotter/material.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 21:36:57.168985 openmc_source_plotter-0.7.1/src/openmc_source_plotter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6511 2024-05-10 21:36:57.000000 openmc_source_plotter-0.7.1/src/openmc_source_plotter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-05-10 21:36:57.000000 openmc_source_plotter-0.7.1/src/openmc_source_plotter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 21:36:57.000000 openmc_source_plotter-0.7.1/src/openmc_source_plotter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-10 21:36:57.000000 openmc_source_plotter-0.7.1/src/openmc_source_plotter.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-10 21:36:57.000000 openmc_source_plotter-0.7.1/src/openmc_source_plotter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-10 21:36:57.000000 openmc_source_plotter-0.7.1/src/openmc_source_plotter.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 21:36:57.168985 openmc_source_plotter-0.7.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2689 2024-05-10 21:36:47.000000 openmc_source_plotter-0.7.1/tests/test_core_with_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2512 2024-05-10 21:36:47.000000 openmc_source_plotter-0.7.1/tests/test_core_with_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2842 2024-05-10 21:36:47.000000 openmc_source_plotter-0.7.1/tests/test_core_with_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 21:36:47.000000 openmc_source_plotter-0.7.1/tests/todo.md
```

### Comparing `openmc_source_plotter-0.7.0/.github/workflows/black.yml` & `openmc_source_plotter-0.7.1/.github/workflows/black.yml`

 * *Files identical despite different names*

### Comparing `openmc_source_plotter-0.7.0/.github/workflows/ci_with_install.yml` & `openmc_source_plotter-0.7.1/.github/workflows/ci_with_install.yml`

 * *Files identical despite different names*

### Comparing `openmc_source_plotter-0.7.0/.github/workflows/lint.yaml` & `openmc_source_plotter-0.7.1/.github/workflows/lint.yaml`

 * *Files identical despite different names*

### Comparing `openmc_source_plotter-0.7.0/.github/workflows/python-publish.yml` & `openmc_source_plotter-0.7.1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `openmc_source_plotter-0.7.0/.gitignore` & `openmc_source_plotter-0.7.1/.gitignore`

 * *Files identical despite different names*

### Comparing `openmc_source_plotter-0.7.0/LICENSE.txt` & `openmc_source_plotter-0.7.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `openmc_source_plotter-0.7.0/PKG-INFO` & `openmc_source_plotter-0.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openmc_source_plotter
-Version: 0.7.0
+Version: 0.7.1
 Summary: A Python package for extracting and plotting the locations, directions, energy distributions of OpenMC source particles.
 Author-email: Jonathan Shimwell <mail@jshimwell.com>
 License: MIT License
         
         Copyright (c) 2021 Fusion Energy
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `openmc_source_plotter-0.7.0/README.md` & `openmc_source_plotter-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `openmc_source_plotter-0.7.0/examples/example_gamma_spec_plot.py` & `openmc_source_plotter-0.7.1/examples/example_gamma_spec_plot.py`

 * *Files identical despite different names*

### Comparing `openmc_source_plotter-0.7.0/examples/example_get_particle_data.py` & `openmc_source_plotter-0.7.1/examples/example_get_particle_data.py`

 * *Files identical despite different names*

### Comparing `openmc_source_plotter-0.7.0/examples/example_plot_plasma_source_position.py` & `openmc_source_plotter-0.7.1/examples/example_plot_plasma_source_position.py`

 * *Files identical despite different names*

### Comparing `openmc_source_plotter-0.7.0/examples/example_plot_source_position.py` & `openmc_source_plotter-0.7.1/examples/example_plot_source_position.py`

 * *Files identical despite different names*

### Comparing `openmc_source_plotter-0.7.0/examples/example_plot_two_source_energies.py` & `openmc_source_plotter-0.7.1/examples/example_plot_two_source_energies.py`

 * *Files identical despite different names*

### Comparing `openmc_source_plotter-0.7.0/examples/gamma_spec.png` & `openmc_source_plotter-0.7.1/examples/gamma_spec.png`

 * *Files identical despite different names*

### Comparing `openmc_source_plotter-0.7.0/pyproject.toml` & `openmc_source_plotter-0.7.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `openmc_source_plotter-0.7.0/src/openmc_source_plotter/__init__.py` & `openmc_source_plotter-0.7.1/src/openmc_source_plotter/__init__.py`

 * *Files identical despite different names*

### Comparing `openmc_source_plotter-0.7.0/src/openmc_source_plotter/core.py` & `openmc_source_plotter-0.7.1/src/openmc_source_plotter/core.py`

 * *Files identical despite different names*

### Comparing `openmc_source_plotter-0.7.0/src/openmc_source_plotter/material.py` & `openmc_source_plotter-0.7.1/src/openmc_source_plotter/material.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,39 @@
 import openmc
 import matplotlib.pyplot as plt
 
 
+def _get_energy_prob(energy_dis):
+    """gets the energy and probability for different openmc.stats including the
+    openmc.stats.Mixutre which itself is made from openmc.stats"""
+
+    if isinstance(energy_dis, openmc.stats.Mixture):
+        stats = energy_dis.distribution
+        multipliers = energy_dis.probability
+    else:
+        stats = [energy_dis]
+        multipliers = [1.0]
+
+    probs = []
+    en = []
+
+    for stat, multiplier in zip(stats, multipliers):
+
+        for p in stat.p:
+            probs.append(0)
+            probs.append(p * multiplier)
+            probs.append(0)
+        for x in stat.x:
+            en.append(x)
+            en.append(x)
+            en.append(x)
+
+    return en, probs
+
+
 def plot_gamma_emission(
     material,
     label_top: int = None,
 ):
     """makes a plot of the gamma energy spectra for a material. The
     material should contain unstable nuclide which undergo gamma emission
     to produce a plot. Such materials can be made manually or obtained via
@@ -44,45 +72,30 @@
         for entry in possible_energies_to_label:
             energies_to_label.append(entry[2])
             labels.append(entry[0])
 
         probs = []
         en = []
         energy_dis = material.get_decay_photon_energy(clip_tolerance=0.0)
-        for p in energy_dis.p:
-            probs.append(0)
-            probs.append(p)
-            probs.append(0)
-        for x in energy_dis.x:
-            en.append(x)
-            en.append(x)
-            en.append(x)
-        # print(en)
-        # print(probs)
+
+        en, probs = _get_energy_prob(energy_dis)
+
         lineid_plot.plot_line_ids(
             en,
             # material.decay_photon_energy.x,
             probs,
             # material.decay_photon_energy.p,
             energies_to_label,
             labels,
         )
 
     else:
-        probs = []
-        en = []
         energy_dis = material.get_decay_photon_energy(clip_tolerance=0.0)
-        for p in energy_dis.p:
-            probs.append(0)
-            probs.append(p)
-            probs.append(0)
-        for x in energy_dis.x:
-            en.append(x)
-            en.append(x)
-            en.append(x)
+
+        en, probs = _get_energy_prob(energy_dis)
 
         # plt.scatter(energy_dis.x, energy_dis.p)
         plt.plot(en, probs)
         # print(energy_dis.p)
         # print(energy_dis.x)
     plt.xlabel("Energy [eV]")
     plt.ylabel("Activity [Bq/s]")
```

### Comparing `openmc_source_plotter-0.7.0/src/openmc_source_plotter.egg-info/PKG-INFO` & `openmc_source_plotter-0.7.1/src/openmc_source_plotter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openmc_source_plotter
-Version: 0.7.0
+Version: 0.7.1
 Summary: A Python package for extracting and plotting the locations, directions, energy distributions of OpenMC source particles.
 Author-email: Jonathan Shimwell <mail@jshimwell.com>
 License: MIT License
         
         Copyright (c) 2021 Fusion Energy
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `openmc_source_plotter-0.7.0/src/openmc_source_plotter.egg-info/SOURCES.txt` & `openmc_source_plotter-0.7.1/src/openmc_source_plotter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openmc_source_plotter-0.7.0/tests/test_core_with_model.py` & `openmc_source_plotter-0.7.1/tests/test_core_with_model.py`

 * *Files identical despite different names*

### Comparing `openmc_source_plotter-0.7.0/tests/test_core_with_settings.py` & `openmc_source_plotter-0.7.1/tests/test_core_with_settings.py`

 * *Files identical despite different names*

### Comparing `openmc_source_plotter-0.7.0/tests/test_core_with_source.py` & `openmc_source_plotter-0.7.1/tests/test_core_with_source.py`

 * *Files identical despite different names*

