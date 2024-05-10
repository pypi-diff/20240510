# Comparing `tmp/MDCraft-0.0.1.tar.gz` & `tmp/mdcraft-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MDCraft-0.0.1.tar", last modified: Mon Mar  4 04:09:42 2024, max compression
+gzip compressed data, was "mdcraft-1.0.0.tar", last modified: Thu May  9 23:52:08 2024, max compression
```

## Comparing `MDCraft-0.0.1.tar` & `mdcraft-1.0.0.tar`

### file list

```diff
@@ -1,15 +1,72 @@
-drwxrwxrwx   0 bye       (1000) bye       (1000)        0 2024-03-04 04:09:50.290804 MDCraft-0.0.1/
--rwxrwxrwx   0 bye       (1000) bye       (1000)        0 2024-03-04 04:08:36.000000 MDCraft-0.0.1/LICENSE
--rwxrwxrwx   0 bye       (1000) bye       (1000)      887 2024-03-04 04:09:50.285296 MDCraft-0.0.1/PKG-INFO
--rwxrwxrwx   0 bye       (1000) bye       (1000)        0 2024-03-04 04:08:43.000000 MDCraft-0.0.1/README.md
--rwxrwxrwx   0 bye       (1000) bye       (1000)      974 2024-03-04 04:06:59.000000 MDCraft-0.0.1/pyproject.toml
--rwxrwxrwx   0 bye       (1000) bye       (1000)       38 2024-03-04 04:09:50.291808 MDCraft-0.0.1/setup.cfg
-drwxrwxrwx   0 bye       (1000) bye       (1000)        0 2024-03-04 04:09:50.152493 MDCraft-0.0.1/src/
-drwxrwxrwx   0 bye       (1000) bye       (1000)        0 2024-03-04 04:09:50.278788 MDCraft-0.0.1/src/MDCraft.egg-info/
--rwxrwxrwx   0 bye       (1000) bye       (1000)      887 2024-03-04 04:09:50.000000 MDCraft-0.0.1/src/MDCraft.egg-info/PKG-INFO
--rwxrwxrwx   0 bye       (1000) bye       (1000)      230 2024-03-04 04:09:50.000000 MDCraft-0.0.1/src/MDCraft.egg-info/SOURCES.txt
--rwxrwxrwx   0 bye       (1000) bye       (1000)        1 2024-03-04 04:09:50.000000 MDCraft-0.0.1/src/MDCraft.egg-info/dependency_links.txt
--rwxrwxrwx   0 bye       (1000) bye       (1000)       60 2024-03-04 04:09:50.000000 MDCraft-0.0.1/src/MDCraft.egg-info/requires.txt
--rwxrwxrwx   0 bye       (1000) bye       (1000)        8 2024-03-04 04:09:50.000000 MDCraft-0.0.1/src/MDCraft.egg-info/top_level.txt
-drwxrwxrwx   0 bye       (1000) bye       (1000)        0 2024-03-04 04:09:50.260690 MDCraft-0.0.1/src/mdcraft/
--rwxrwxrwx   0 bye       (1000) bye       (1000)        0 2024-03-04 04:08:16.000000 MDCraft-0.0.1/src/mdcraft/__init__.py
+drwxrwxrwx   0 bye       (1000) bye       (1000)        0 2024-05-09 23:52:12.381265 mdcraft-1.0.0/
+-rwxrwxrwx   0 bye       (1000) bye       (1000)    35149 2024-05-07 05:37:14.000000 mdcraft-1.0.0/LICENSE
+-rwxrwxrwx   0 bye       (1000) bye       (1000)    44462 2024-05-09 23:52:12.375168 mdcraft-1.0.0/PKG-INFO
+-rwxrwxrwx   0 bye       (1000) bye       (1000)     3039 2024-05-09 23:49:19.000000 mdcraft-1.0.0/README.md
+-rwxrwxrwx   0 bye       (1000) bye       (1000)      931 2024-05-07 05:44:25.000000 mdcraft-1.0.0/pyproject.toml
+-rwxrwxrwx   0 bye       (1000) bye       (1000)       38 2024-05-09 23:52:12.381265 mdcraft-1.0.0/setup.cfg
+drwxrwxrwx   0 bye       (1000) bye       (1000)        0 2024-05-09 23:52:11.213199 mdcraft-1.0.0/src/
+drwxrwxrwx   0 bye       (1000) bye       (1000)        0 2024-05-09 23:52:11.302046 mdcraft-1.0.0/src/mdcraft/
+-rwxrwxrwx   0 bye       (1000) bye       (1000)      445 2024-05-09 22:50:39.000000 mdcraft-1.0.0/src/mdcraft/__init__.py
+drwxrwxrwx   0 bye       (1000) bye       (1000)        0 2024-05-09 23:52:11.536562 mdcraft-1.0.0/src/mdcraft/algorithm/
+-rwxrwxrwx   0 bye       (1000) bye       (1000)      327 2024-05-08 05:09:35.000000 mdcraft-1.0.0/src/mdcraft/algorithm/__init__.py
+-rwxrwxrwx   0 bye       (1000) bye       (1000)    15387 2024-05-09 23:27:09.000000 mdcraft-1.0.0/src/mdcraft/algorithm/accelerated.py
+-rwxrwxrwx   0 bye       (1000) bye       (1000)    30777 2024-05-09 23:12:14.000000 mdcraft-1.0.0/src/mdcraft/algorithm/correlation.py
+-rwxrwxrwx   0 bye       (1000) bye       (1000)    24007 2024-05-09 22:27:35.000000 mdcraft-1.0.0/src/mdcraft/algorithm/molecule.py
+-rwxrwxrwx   0 bye       (1000) bye       (1000)    20388 2024-05-09 22:32:06.000000 mdcraft-1.0.0/src/mdcraft/algorithm/topology.py
+-rwxrwxrwx   0 bye       (1000) bye       (1000)    10787 2024-05-09 22:45:00.000000 mdcraft-1.0.0/src/mdcraft/algorithm/unit.py
+-rwxrwxrwx   0 bye       (1000) bye       (1000)     5469 2024-05-09 23:29:46.000000 mdcraft-1.0.0/src/mdcraft/algorithm/utility.py
+drwxrwxrwx   0 bye       (1000) bye       (1000)        0 2024-05-09 23:52:11.703168 mdcraft-1.0.0/src/mdcraft/analysis/
+-rwxrwxrwx   0 bye       (1000) bye       (1000)      423 2024-05-09 22:46:51.000000 mdcraft-1.0.0/src/mdcraft/analysis/__init__.py
+-rwxrwxrwx   0 bye       (1000) bye       (1000)    19958 2024-05-09 22:46:51.000000 mdcraft-1.0.0/src/mdcraft/analysis/base.py
+-rwxrwxrwx   0 bye       (1000) bye       (1000)    18531 2024-05-09 22:46:52.000000 mdcraft-1.0.0/src/mdcraft/analysis/electrostatics.py
+-rwxrwxrwx   0 bye       (1000) bye       (1000)    43974 2024-05-09 23:06:32.000000 mdcraft-1.0.0/src/mdcraft/analysis/polymer.py
+-rwxrwxrwx   0 bye       (1000) bye       (1000)    39225 2024-05-09 22:46:52.000000 mdcraft-1.0.0/src/mdcraft/analysis/profile.py
+-rwxrwxrwx   0 bye       (1000) bye       (1000)    80388 2024-05-09 22:46:52.000000 mdcraft-1.0.0/src/mdcraft/analysis/structure.py
+-rwxrwxrwx   0 bye       (1000) bye       (1000)     9299 2024-05-09 22:46:52.000000 mdcraft-1.0.0/src/mdcraft/analysis/thermodynamics.py
+-rwxrwxrwx   0 bye       (1000) bye       (1000)    50420 2024-05-09 23:18:32.000000 mdcraft-1.0.0/src/mdcraft/analysis/transport.py
+drwxrwxrwx   0 bye       (1000) bye       (1000)        0 2024-05-09 23:52:11.861690 mdcraft-1.0.0/src/mdcraft/fit/
+-rwxrwxrwx   0 bye       (1000) bye       (1000)      437 2024-05-09 22:47:03.000000 mdcraft-1.0.0/src/mdcraft/fit/__init__.py
+-rwxrwxrwx   0 bye       (1000) bye       (1000)     1992 2024-05-09 22:47:03.000000 mdcraft-1.0.0/src/mdcraft/fit/distribution.py
+-rwxrwxrwx   0 bye       (1000) bye       (1000)     6139 2024-05-09 22:47:03.000000 mdcraft-1.0.0/src/mdcraft/fit/exponential.py
+-rwxrwxrwx   0 bye       (1000) bye       (1000)    15855 2024-05-09 22:47:03.000000 mdcraft-1.0.0/src/mdcraft/fit/fourier.py
+-rwxrwxrwx   0 bye       (1000) bye       (1000)    16773 2024-05-09 22:47:03.000000 mdcraft-1.0.0/src/mdcraft/fit/gaussian.py
+-rwxrwxrwx   0 bye       (1000) bye       (1000)    10566 2024-05-09 22:47:03.000000 mdcraft-1.0.0/src/mdcraft/fit/polynomial.py
+-rwxrwxrwx   0 bye       (1000) bye       (1000)     2012 2024-05-09 22:47:03.000000 mdcraft-1.0.0/src/mdcraft/fit/power.py
+drwxrwxrwx   0 bye       (1000) bye       (1000)        0 2024-05-09 23:52:11.906201 mdcraft-1.0.0/src/mdcraft/lammps/
+-rwxrwxrwx   0 bye       (1000) bye       (1000)      208 2024-05-09 22:47:38.000000 mdcraft-1.0.0/src/mdcraft/lammps/__init__.py
+-rwxrwxrwx   0 bye       (1000) bye       (1000)     7105 2024-05-09 23:31:08.000000 mdcraft-1.0.0/src/mdcraft/lammps/topology.py
+drwxrwxrwx   0 bye       (1000) bye       (1000)        0 2024-05-09 23:52:12.101087 mdcraft-1.0.0/src/mdcraft/openmm/
+-rwxrwxrwx   0 bye       (1000) bye       (1000)      335 2024-05-09 22:47:49.000000 mdcraft-1.0.0/src/mdcraft/openmm/__init__.py
+-rwxrwxrwx   0 bye       (1000) bye       (1000)     3579 2024-05-09 23:06:32.000000 mdcraft-1.0.0/src/mdcraft/openmm/bond.py
+-rwxrwxrwx   0 bye       (1000) bye       (1000)    24149 2024-05-09 23:06:40.000000 mdcraft-1.0.0/src/mdcraft/openmm/file.py
+-rwxrwxrwx   0 bye       (1000) bye       (1000)    49089 2024-05-09 22:47:49.000000 mdcraft-1.0.0/src/mdcraft/openmm/pair.py
+-rwxrwxrwx   0 bye       (1000) bye       (1000)     6367 2024-05-09 22:47:49.000000 mdcraft-1.0.0/src/mdcraft/openmm/reporter.py
+-rwxrwxrwx   0 bye       (1000) bye       (1000)    43384 2024-05-09 23:31:35.000000 mdcraft-1.0.0/src/mdcraft/openmm/system.py
+-rwxrwxrwx   0 bye       (1000) bye       (1000)     8714 2024-05-09 23:06:31.000000 mdcraft-1.0.0/src/mdcraft/openmm/topology.py
+-rwxrwxrwx   0 bye       (1000) bye       (1000)     1139 2024-05-09 22:37:55.000000 mdcraft-1.0.0/src/mdcraft/openmm/unit.py
+-rwxrwxrwx   0 bye       (1000) bye       (1000)    11993 2024-05-09 23:31:51.000000 mdcraft-1.0.0/src/mdcraft/openmm/utility.py
+drwxrwxrwx   0 bye       (1000) bye       (1000)        0 2024-05-09 23:52:12.191606 mdcraft-1.0.0/src/mdcraft/plot/
+-rwxrwxrwx   0 bye       (1000) bye       (1000)      297 2024-05-09 23:20:35.000000 mdcraft-1.0.0/src/mdcraft/plot/__init__.py
+-rwxrwxrwx   0 bye       (1000) bye       (1000)     4388 2024-05-09 22:48:10.000000 mdcraft-1.0.0/src/mdcraft/plot/axis.py
+-rwxrwxrwx   0 bye       (1000) bye       (1000)     1495 2024-05-09 22:48:10.000000 mdcraft-1.0.0/src/mdcraft/plot/color.py
+-rwxrwxrwx   0 bye       (1000) bye       (1000)     3090 2024-05-09 23:21:07.000000 mdcraft-1.0.0/src/mdcraft/plot/rcparam.py
+drwxrwxrwx   0 bye       (1000) bye       (1000)        0 2024-05-09 23:52:12.367000 mdcraft-1.0.0/src/mdcraft.egg-info/
+-rwxrwxrwx   0 bye       (1000) bye       (1000)    44462 2024-05-09 23:52:10.000000 mdcraft-1.0.0/src/mdcraft.egg-info/PKG-INFO
+-rwxrwxrwx   0 bye       (1000) bye       (1000)     1792 2024-05-09 23:52:11.000000 mdcraft-1.0.0/src/mdcraft.egg-info/SOURCES.txt
+-rwxrwxrwx   0 bye       (1000) bye       (1000)        1 2024-05-09 23:52:10.000000 mdcraft-1.0.0/src/mdcraft.egg-info/dependency_links.txt
+-rwxrwxrwx   0 bye       (1000) bye       (1000)       66 2024-05-09 23:52:10.000000 mdcraft-1.0.0/src/mdcraft.egg-info/requires.txt
+-rwxrwxrwx   0 bye       (1000) bye       (1000)        8 2024-05-09 23:52:10.000000 mdcraft-1.0.0/src/mdcraft.egg-info/top_level.txt
+drwxrwxrwx   0 bye       (1000) bye       (1000)        0 2024-05-09 23:52:12.348993 mdcraft-1.0.0/tests/
+-rwxrwxrwx   0 bye       (1000) bye       (1000)    20598 2024-05-09 23:06:31.000000 mdcraft-1.0.0/tests/test_algorithm_correlation.py
+-rwxrwxrwx   0 bye       (1000) bye       (1000)     6638 2024-05-09 23:06:31.000000 mdcraft-1.0.0/tests/test_algorithm_molecule.py
+-rwxrwxrwx   0 bye       (1000) bye       (1000)     4655 2024-05-09 23:14:02.000000 mdcraft-1.0.0/tests/test_algorithm_topology.py
+-rwxrwxrwx   0 bye       (1000) bye       (1000)     2999 2024-05-09 23:06:31.000000 mdcraft-1.0.0/tests/test_algorithm_unit.py
+-rwxrwxrwx   0 bye       (1000) bye       (1000)     1529 2024-05-09 23:06:31.000000 mdcraft-1.0.0/tests/test_algorithm_utility.py
+-rwxrwxrwx   0 bye       (1000) bye       (1000)     1156 2024-05-09 23:06:31.000000 mdcraft-1.0.0/tests/test_analysis_electrostatics.py
+-rwxrwxrwx   0 bye       (1000) bye       (1000)     2288 2024-05-09 23:06:31.000000 mdcraft-1.0.0/tests/test_analysis_polymer.py
+-rwxrwxrwx   0 bye       (1000) bye       (1000)     1830 2024-05-09 23:06:31.000000 mdcraft-1.0.0/tests/test_analysis_profile.py
+-rwxrwxrwx   0 bye       (1000) bye       (1000)    12175 2024-05-09 23:06:31.000000 mdcraft-1.0.0/tests/test_analysis_structure.py
+-rwxrwxrwx   0 bye       (1000) bye       (1000)     7377 2024-05-09 23:06:31.000000 mdcraft-1.0.0/tests/test_analysis_transport.py
+-rwxrwxrwx   0 bye       (1000) bye       (1000)     5504 2024-05-09 23:06:40.000000 mdcraft-1.0.0/tests/test_openmm_file_reporter.py
+-rwxrwxrwx   0 bye       (1000) bye       (1000)     3669 2024-05-09 23:06:31.000000 mdcraft-1.0.0/tests/test_openmm_topology.py
+-rwxrwxrwx   0 bye       (1000) bye       (1000)     1318 2024-05-09 23:06:31.000000 mdcraft-1.0.0/tests/test_openmm_unit.py
```

### Comparing `MDCraft-0.0.1/pyproject.toml` & `mdcraft-1.0.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,39 +1,38 @@
 [build-system]
 build-backend = "setuptools.build_meta"
 requires = ["setuptools"]
 
 [project]
-name = "MDCraft"
-version = "0.0.1"
+name = "mdcraft"
+version = "1.0.0"
 authors = [
   { name = "Benjamin B. Ye", email = "bye@caltech.edu" },
   { name = "Pierre J. Walker", email = "pjwalker@caltech.edu" },
+  { name = "Alec G. Glisman", email = "aglisman@caltech.edu" }
 ]
 classifiers = [
   "Intended Audience :: Science/Research",
   "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
   "Operating System :: OS Independent",
   "Programming Language :: Python",
   "Programming Language :: Python :: 3"
 ]
 dependencies = [
   "matplotlib",
   "mdanalysis",
   "netCDF4",
+  "numba",
   "numpy",
   "pandas",
   "pint",
   "scipy",
   "sympy"
 ]
-description = """
-A batteries-included toolkit of analysis modules and helper functions 
-for molecular dynamics (MD) simulations.
-"""
+description = ""
 license = { file = "LICENSE" }
 readme = "README.md"
 requires-python = ">=3.9"
 
 [project.urls]
 "Homepage" = "https://github.com/bbye98/mdcraft"
 "Bug Tracker" = "https://github.com/bbye98/mdcraft/issues"
```

