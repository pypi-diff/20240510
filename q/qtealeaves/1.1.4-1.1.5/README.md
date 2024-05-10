# Comparing `tmp/qtealeaves-1.1.4.tar.gz` & `tmp/qtealeaves-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qtealeaves-1.1.4.tar", last modified: Thu May  9 07:06:24 2024, max compression
+gzip compressed data, was "qtealeaves-1.1.5.tar", last modified: Fri May 10 15:06:53 2024, max compression
```

## Comparing `qtealeaves-1.1.4.tar` & `qtealeaves-1.1.5.tar`

### file list

```diff
@@ -1,112 +1,112 @@
-drwxr-xr-x   0 quantum    (128) quantum    (128)        0 2024-05-09 07:06:24.253241 qtealeaves-1.1.4/
--rw-r--r--   0 quantum    (128) quantum    (128)    10764 2022-11-30 17:54:07.000000 qtealeaves-1.1.4/LICENSE
--rw-r--r--   0 quantum    (128) quantum    (128)     3319 2024-05-09 07:06:24.253241 qtealeaves-1.1.4/PKG-INFO
--rw-r--r--   0 quantum    (128) quantum    (128)     2572 2023-12-13 17:32:06.000000 qtealeaves-1.1.4/README.md
--rw-r--r--   0 quantum    (128) quantum    (128)      101 2024-04-19 13:19:04.000000 qtealeaves-1.1.4/pyproject.toml
-drwxr-xr-x   0 quantum    (128) quantum    (128)        0 2024-05-09 07:06:24.245241 qtealeaves-1.1.4/qtealeaves/
--rw-r--r--   0 quantum    (128) quantum    (128)     1088 2024-04-19 13:19:04.000000 qtealeaves-1.1.4/qtealeaves/__init__.py
-drwxr-xr-x   0 quantum    (128) quantum    (128)        0 2024-05-09 07:06:24.245241 qtealeaves-1.1.4/qtealeaves/convergence_parameters/
--rw-r--r--   0 quantum    (128) quantum    (128)      758 2022-11-30 17:54:07.000000 qtealeaves-1.1.4/qtealeaves/convergence_parameters/__init__.py
--rw-r--r--   0 quantum    (128) quantum    (128)    20340 2024-04-19 13:19:04.000000 qtealeaves-1.1.4/qtealeaves/convergence_parameters/conv_params.py
--rw-r--r--   0 quantum    (128) quantum    (128)     6745 2024-01-12 22:24:30.000000 qtealeaves-1.1.4/qtealeaves/convergence_parameters/conv_params_finite_temp.py
-drwxr-xr-x   0 quantum    (128) quantum    (128)        0 2024-05-09 07:06:24.245241 qtealeaves-1.1.4/qtealeaves/emulator/
--rw-r--r--   0 quantum    (128) quantum    (128)     1485 2024-04-19 13:19:04.000000 qtealeaves-1.1.4/qtealeaves/emulator/__init__.py
--rw-r--r--   0 quantum    (128) quantum    (128)    89623 2024-05-09 06:53:17.000000 qtealeaves-1.1.4/qtealeaves/emulator/abstract_tn.py
--rw-r--r--   0 quantum    (128) quantum    (128)    13132 2024-04-19 13:19:04.000000 qtealeaves-1.1.4/qtealeaves/emulator/attn_simulator.py
--rw-r--r--   0 quantum    (128) quantum    (128)     9504 2024-04-19 13:19:04.000000 qtealeaves-1.1.4/qtealeaves/emulator/ed_simulation.py
--rw-r--r--   0 quantum    (128) quantum    (128)    42373 2024-05-09 06:53:17.000000 qtealeaves-1.1.4/qtealeaves/emulator/lptn_simulator.py
--rw-r--r--   0 quantum    (128) quantum    (128)    22203 2024-05-09 06:53:17.000000 qtealeaves-1.1.4/qtealeaves/emulator/mpi_mps_simulator.py
--rw-r--r--   0 quantum    (128) quantum    (128)   111015 2024-05-09 06:53:17.000000 qtealeaves-1.1.4/qtealeaves/emulator/mps_simulator.py
--rw-r--r--   0 quantum    (128) quantum    (128)    19742 2024-04-19 13:19:04.000000 qtealeaves-1.1.4/qtealeaves/emulator/state_simulator.py
--rw-r--r--   0 quantum    (128) quantum    (128)    39482 2024-05-08 11:06:39.000000 qtealeaves-1.1.4/qtealeaves/emulator/tn_simulation.py
--rw-r--r--   0 quantum    (128) quantum    (128)     2535 2024-04-19 13:19:04.000000 qtealeaves-1.1.4/qtealeaves/emulator/tnnode.py
--rw-r--r--   0 quantum    (128) quantum    (128)   168938 2024-05-08 11:06:39.000000 qtealeaves-1.1.4/qtealeaves/emulator/ttn_simulator.py
--rw-r--r--   0 quantum    (128) quantum    (128)    46305 2024-04-19 13:19:04.000000 qtealeaves-1.1.4/qtealeaves/emulator/tto_simulator.py
--rw-r--r--   0 quantum    (128) quantum    (128)     2125 2024-04-19 13:19:04.000000 qtealeaves-1.1.4/qtealeaves/emulator/unitariesprojmeas.py
-drwxr-xr-x   0 quantum    (128) quantum    (128)        0 2024-05-09 07:06:24.245241 qtealeaves-1.1.4/qtealeaves/modeling/
--rw-r--r--   0 quantum    (128) quantum    (128)     1289 2024-04-19 13:19:04.000000 qtealeaves-1.1.4/qtealeaves/modeling/__init__.py
--rw-r--r--   0 quantum    (128) quantum    (128)     6956 2024-04-19 13:19:04.000000 qtealeaves-1.1.4/qtealeaves/modeling/baseterm.py
--rw-r--r--   0 quantum    (128) quantum    (128)     7625 2024-04-19 13:19:04.000000 qtealeaves-1.1.4/qtealeaves/modeling/blockterm2d.py
--rw-r--r--   0 quantum    (128) quantum    (128)    16787 2024-04-19 13:19:04.000000 qtealeaves-1.1.4/qtealeaves/modeling/localterm.py
--rw-r--r--   0 quantum    (128) quantum    (128)     7379 2024-04-19 13:19:04.000000 qtealeaves-1.1.4/qtealeaves/modeling/plaquetteterm2d.py
--rw-r--r--   0 quantum    (128) quantum    (128)    32850 2024-04-19 13:19:04.000000 qtealeaves-1.1.4/qtealeaves/modeling/quantummodel.py
--rw-r--r--   0 quantum    (128) quantum    (128)     5632 2024-02-26 14:55:43.000000 qtealeaves-1.1.4/qtealeaves/modeling/stringterm1d.py
--rw-r--r--   0 quantum    (128) quantum    (128)    13220 2024-05-09 06:53:17.000000 qtealeaves-1.1.4/qtealeaves/modeling/twobodyterm1d.py
--rw-r--r--   0 quantum    (128) quantum    (128)    13088 2024-04-19 13:19:04.000000 qtealeaves-1.1.4/qtealeaves/modeling/twobodyterm2d.py
--rw-r--r--   0 quantum    (128) quantum    (128)    10657 2024-04-19 13:19:04.000000 qtealeaves-1.1.4/qtealeaves/modeling/twobodyterm3d.py
-drwxr-xr-x   0 quantum    (128) quantum    (128)        0 2024-05-09 07:06:24.245241 qtealeaves-1.1.4/qtealeaves/models/
--rw-r--r--   0 quantum    (128) quantum    (128)      766 2022-11-30 17:54:07.000000 qtealeaves-1.1.4/qtealeaves/models/__init__.py
--rw-r--r--   0 quantum    (128) quantum    (128)     2720 2022-11-30 17:54:07.000000 qtealeaves-1.1.4/qtealeaves/models/bosehubbard.py
--rw-r--r--   0 quantum    (128) quantum    (128)     4682 2023-10-26 07:55:27.000000 qtealeaves-1.1.4/qtealeaves/models/quantumising.py
--rw-r--r--   0 quantum    (128) quantum    (128)     1736 2022-11-30 17:54:07.000000 qtealeaves-1.1.4/qtealeaves/models/xxzmodel.py
-drwxr-xr-x   0 quantum    (128) quantum    (128)        0 2024-05-09 07:06:24.249241 qtealeaves-1.1.4/qtealeaves/mpos/
--rw-r--r--   0 quantum    (128) quantum    (128)     1239 2024-04-19 13:19:04.000000 qtealeaves-1.1.4/qtealeaves/mpos/__init__.py
--rw-r--r--   0 quantum    (128) quantum    (128)     4018 2024-04-19 13:19:04.000000 qtealeaves-1.1.4/qtealeaves/mpos/abstracteffop.py
--rw-r--r--   0 quantum    (128) quantum    (128)    15982 2024-04-19 13:19:04.000000 qtealeaves-1.1.4/qtealeaves/mpos/densempos.py
--rw-r--r--   0 quantum    (128) quantum    (128)    15908 2024-04-19 13:19:04.000000 qtealeaves-1.1.4/qtealeaves/mpos/disentangler.py
--rw-r--r--   0 quantum    (128) quantum    (128)    76751 2024-04-19 13:19:04.000000 qtealeaves-1.1.4/qtealeaves/mpos/indexedtpo.py
--rw-r--r--   0 quantum    (128) quantum    (128)    23290 2024-04-19 13:19:04.000000 qtealeaves-1.1.4/qtealeaves/mpos/sparsematrixoperator.py
--rw-r--r--   0 quantum    (128) quantum    (128)    20242 2024-04-19 13:19:04.000000 qtealeaves-1.1.4/qtealeaves/mpos/sparsematrixproductoperator.py
--rw-r--r--   0 quantum    (128) quantum    (128)    21798 2024-04-19 13:19:04.000000 qtealeaves-1.1.4/qtealeaves/mpos/tensorproductoperator.py
-drwxr-xr-x   0 quantum    (128) quantum    (128)        0 2024-05-09 07:06:24.249241 qtealeaves-1.1.4/qtealeaves/observables/
--rw-r--r--   0 quantum    (128) quantum    (128)     1530 2024-01-12 22:24:30.000000 qtealeaves-1.1.4/qtealeaves/observables/__init__.py
--rw-r--r--   0 quantum    (128) quantum    (128)     6009 2024-04-19 13:19:04.000000 qtealeaves-1.1.4/qtealeaves/observables/bond_entropy.py
--rw-r--r--   0 quantum    (128) quantum    (128)    19724 2024-04-19 13:19:04.000000 qtealeaves-1.1.4/qtealeaves/observables/correlation.py
--rw-r--r--   0 quantum    (128) quantum    (128)    12681 2024-04-19 13:19:04.000000 qtealeaves-1.1.4/qtealeaves/observables/custom_correlation.py
--rw-r--r--   0 quantum    (128) quantum    (128)     4703 2024-04-19 13:19:04.000000 qtealeaves-1.1.4/qtealeaves/observables/distance2pure.py
--rw-r--r--   0 quantum    (128) quantum    (128)     5908 2024-04-19 13:19:04.000000 qtealeaves-1.1.4/qtealeaves/observables/local.py
--rw-r--r--   0 quantum    (128) quantum    (128)     7874 2024-04-19 13:19:04.000000 qtealeaves-1.1.4/qtealeaves/observables/probabilities.py
--rw-r--r--   0 quantum    (128) quantum    (128)     5653 2024-04-19 13:19:04.000000 qtealeaves-1.1.4/qtealeaves/observables/projective.py
--rw-r--r--   0 quantum    (128) quantum    (128)     5110 2024-04-19 13:19:04.000000 qtealeaves-1.1.4/qtealeaves/observables/state2file.py
--rw-r--r--   0 quantum    (128) quantum    (128)     5834 2024-04-19 13:19:04.000000 qtealeaves-1.1.4/qtealeaves/observables/tensor_product.py
--rw-r--r--   0 quantum    (128) quantum    (128)     5609 2024-04-19 13:19:04.000000 qtealeaves-1.1.4/qtealeaves/observables/timecorrelator.py
--rw-r--r--   0 quantum    (128) quantum    (128)     6351 2024-04-19 13:19:04.000000 qtealeaves-1.1.4/qtealeaves/observables/tnobase.py
--rw-r--r--   0 quantum    (128) quantum    (128)    18721 2024-04-19 13:19:04.000000 qtealeaves-1.1.4/qtealeaves/observables/tnobservables.py
--rw-r--r--   0 quantum    (128) quantum    (128)    10161 2024-04-19 13:19:04.000000 qtealeaves-1.1.4/qtealeaves/observables/weighted_sum.py
-drwxr-xr-x   0 quantum    (128) quantum    (128)        0 2024-05-09 07:06:24.249241 qtealeaves-1.1.4/qtealeaves/operators/
--rw-r--r--   0 quantum    (128) quantum    (128)     1004 2023-10-26 07:55:27.000000 qtealeaves-1.1.4/qtealeaves/operators/__init__.py
--rw-r--r--   0 quantum    (128) quantum    (128)     2894 2024-04-19 13:19:04.000000 qtealeaves-1.1.4/qtealeaves/operators/bosonicoperators.py
--rw-r--r--   0 quantum    (128) quantum    (128)     2620 2024-05-02 13:16:14.000000 qtealeaves-1.1.4/qtealeaves/operators/combinedoperators.py
--rw-r--r--   0 quantum    (128) quantum    (128)     4143 2022-11-30 17:54:07.000000 qtealeaves-1.1.4/qtealeaves/operators/quditoperators.py
--rw-r--r--   0 quantum    (128) quantum    (128)     1368 2024-04-19 13:19:04.000000 qtealeaves-1.1.4/qtealeaves/operators/spinoperators.py
--rw-r--r--   0 quantum    (128) quantum    (128)     9216 2024-04-19 13:19:04.000000 qtealeaves-1.1.4/qtealeaves/operators/tnoperators.py
--rw-r--r--   0 quantum    (128) quantum    (128)    68904 2024-04-19 13:19:04.000000 qtealeaves-1.1.4/qtealeaves/simulation_setup.py
-drwxr-xr-x   0 quantum    (128) quantum    (128)        0 2024-05-09 07:06:24.249241 qtealeaves-1.1.4/qtealeaves/solvers/
--rw-r--r--   0 quantum    (128) quantum    (128)      698 2024-04-19 13:19:04.000000 qtealeaves-1.1.4/qtealeaves/solvers/__init__.py
--rw-r--r--   0 quantum    (128) quantum    (128)     4067 2024-04-19 13:19:04.000000 qtealeaves-1.1.4/qtealeaves/solvers/eigen_solver.py
--rw-r--r--   0 quantum    (128) quantum    (128)     7352 2024-04-19 13:19:04.000000 qtealeaves-1.1.4/qtealeaves/solvers/krylovexp_solver.py
-drwxr-xr-x   0 quantum    (128) quantum    (128)        0 2024-05-09 07:06:24.249241 qtealeaves-1.1.4/qtealeaves/tensors/
--rw-r--r--   0 quantum    (128) quantum    (128)      801 2024-04-19 13:19:04.000000 qtealeaves-1.1.4/qtealeaves/tensors/__init__.py
--rw-r--r--   0 quantum    (128) quantum    (128)    17043 2024-04-19 13:19:04.000000 qtealeaves-1.1.4/qtealeaves/tensors/abstracttensor.py
--rw-r--r--   0 quantum    (128) quantum    (128)    75600 2024-05-09 06:53:17.000000 qtealeaves-1.1.4/qtealeaves/tensors/tensor.py
--rw-r--r--   0 quantum    (128) quantum    (128)     1663 2024-04-19 13:19:04.000000 qtealeaves-1.1.4/qtealeaves/tensors/tensor_backend.py
-drwxr-xr-x   0 quantum    (128) quantum    (128)        0 2024-05-09 07:06:24.249241 qtealeaves-1.1.4/qtealeaves/tooling/
--rw-r--r--   0 quantum    (128) quantum    (128)     1179 2024-04-19 13:19:04.000000 qtealeaves-1.1.4/qtealeaves/tooling/__init__.py
--rw-r--r--   0 quantum    (128) quantum    (128)    17831 2024-04-19 13:19:04.000000 qtealeaves-1.1.4/qtealeaves/tooling/fortran_interfaces.py
--rw-r--r--   0 quantum    (128) quantum    (128)    47759 2024-04-19 13:19:04.000000 qtealeaves-1.1.4/qtealeaves/tooling/hilbert_curvature.py
--rw-r--r--   0 quantum    (128) quantum    (128)     5883 2024-04-19 13:19:04.000000 qtealeaves-1.1.4/qtealeaves/tooling/lattice_layout.py
--rw-r--r--   0 quantum    (128) quantum    (128)     4080 2024-04-19 13:19:04.000000 qtealeaves-1.1.4/qtealeaves/tooling/parameterized.py
--rw-r--r--   0 quantum    (128) quantum    (128)     1768 2024-04-19 13:19:04.000000 qtealeaves-1.1.4/qtealeaves/tooling/permutations.py
--rw-r--r--   0 quantum    (128) quantum    (128)     1785 2024-04-19 13:19:04.000000 qtealeaves-1.1.4/qtealeaves/tooling/restrictedclasses.py
--rw-r--r--   0 quantum    (128) quantum    (128)      531 2024-05-09 06:53:17.000000 qtealeaves-1.1.4/qtealeaves/version.py
-drwxr-xr-x   0 quantum    (128) quantum    (128)        0 2024-05-09 07:06:24.253241 qtealeaves-1.1.4/qtealeaves.egg-info/
--rw-r--r--   0 quantum    (128) quantum    (128)     3319 2024-05-09 07:06:24.000000 qtealeaves-1.1.4/qtealeaves.egg-info/PKG-INFO
--rw-r--r--   0 quantum    (128) quantum    (128)     3297 2024-05-09 07:06:24.000000 qtealeaves-1.1.4/qtealeaves.egg-info/SOURCES.txt
--rw-r--r--   0 quantum    (128) quantum    (128)        1 2024-05-09 07:06:24.000000 qtealeaves-1.1.4/qtealeaves.egg-info/dependency_links.txt
--rw-r--r--   0 quantum    (128) quantum    (128)       42 2024-05-09 07:06:24.000000 qtealeaves-1.1.4/qtealeaves.egg-info/requires.txt
--rw-r--r--   0 quantum    (128) quantum    (128)       11 2024-05-09 07:06:24.000000 qtealeaves-1.1.4/qtealeaves.egg-info/top_level.txt
--rw-r--r--   0 quantum    (128) quantum    (128)       38 2024-05-09 07:06:24.253241 qtealeaves-1.1.4/setup.cfg
--rw-r--r--   0 quantum    (128) quantum    (128)     3041 2024-05-02 13:16:14.000000 qtealeaves-1.1.4/setup.py
-drwxr-xr-x   0 quantum    (128) quantum    (128)        0 2024-05-09 07:06:24.253241 qtealeaves-1.1.4/tests/
--rw-r--r--   0 quantum    (128) quantum    (128)     1332 2022-11-30 17:54:07.000000 qtealeaves-1.1.4/tests/tests_formatting.py
--rw-r--r--   0 quantum    (128) quantum    (128)     1504 2023-10-26 07:55:27.000000 qtealeaves-1.1.4/tests/tests_fortran_interface.py
--rw-r--r--   0 quantum    (128) quantum    (128)     9308 2024-05-09 06:53:17.000000 qtealeaves-1.1.4/tests/tests_hilbert_curvature.py
--rw-r--r--   0 quantum    (128) quantum    (128)     2732 2024-04-19 13:19:04.000000 qtealeaves-1.1.4/tests/tests_lattice_layout.py
--rw-r--r--   0 quantum    (128) quantum    (128)    27539 2024-04-19 13:19:04.000000 qtealeaves-1.1.4/tests/tests_linter.py
--rw-r--r--   0 quantum    (128) quantum    (128)     5818 2023-10-26 07:55:27.000000 qtealeaves-1.1.4/tests/tests_model_terms.py
--rw-r--r--   0 quantum    (128) quantum    (128)     9812 2024-04-19 13:19:04.000000 qtealeaves-1.1.4/tests/tests_observables.py
--rw-r--r--   0 quantum    (128) quantum    (128)     1858 2023-01-26 15:54:33.000000 qtealeaves-1.1.4/tests/tests_operators.py
--rw-r--r--   0 quantum    (128) quantum    (128)     2962 2024-04-19 13:19:04.000000 qtealeaves-1.1.4/tests/tests_quantum_trajectories.py
--rw-r--r--   0 quantum    (128) quantum    (128)     2553 2022-11-30 17:54:07.000000 qtealeaves-1.1.4/tests/tests_rydberg_model.py
--rw-r--r--   0 quantum    (128) quantum    (128)     4401 2024-04-19 13:19:04.000000 qtealeaves-1.1.4/tests/tests_simulation_setup.py
--rw-r--r--   0 quantum    (128) quantum    (128)    14206 2024-05-09 06:53:17.000000 qtealeaves-1.1.4/tests/tests_tn_simulation.py
+drwxr-xr-x   0 quantum    (128) quantum    (128)        0 2024-05-10 15:06:52.995487 qtealeaves-1.1.5/
+-rw-r--r--   0 quantum    (128) quantum    (128)    10764 2022-11-30 17:54:07.000000 qtealeaves-1.1.5/LICENSE
+-rw-r--r--   0 quantum    (128) quantum    (128)     3319 2024-05-10 15:06:52.995487 qtealeaves-1.1.5/PKG-INFO
+-rw-r--r--   0 quantum    (128) quantum    (128)     2572 2023-12-13 17:32:06.000000 qtealeaves-1.1.5/README.md
+-rw-r--r--   0 quantum    (128) quantum    (128)      101 2024-04-19 13:19:04.000000 qtealeaves-1.1.5/pyproject.toml
+drwxr-xr-x   0 quantum    (128) quantum    (128)        0 2024-05-10 15:06:52.987487 qtealeaves-1.1.5/qtealeaves/
+-rw-r--r--   0 quantum    (128) quantum    (128)     1088 2024-04-19 13:19:04.000000 qtealeaves-1.1.5/qtealeaves/__init__.py
+drwxr-xr-x   0 quantum    (128) quantum    (128)        0 2024-05-10 15:06:52.987487 qtealeaves-1.1.5/qtealeaves/convergence_parameters/
+-rw-r--r--   0 quantum    (128) quantum    (128)      758 2022-11-30 17:54:07.000000 qtealeaves-1.1.5/qtealeaves/convergence_parameters/__init__.py
+-rw-r--r--   0 quantum    (128) quantum    (128)    20340 2024-04-19 13:19:04.000000 qtealeaves-1.1.5/qtealeaves/convergence_parameters/conv_params.py
+-rw-r--r--   0 quantum    (128) quantum    (128)     6745 2024-01-12 22:24:30.000000 qtealeaves-1.1.5/qtealeaves/convergence_parameters/conv_params_finite_temp.py
+drwxr-xr-x   0 quantum    (128) quantum    (128)        0 2024-05-10 15:06:52.987487 qtealeaves-1.1.5/qtealeaves/emulator/
+-rw-r--r--   0 quantum    (128) quantum    (128)     1684 2024-05-10 14:53:16.000000 qtealeaves-1.1.5/qtealeaves/emulator/__init__.py
+-rw-r--r--   0 quantum    (128) quantum    (128)    89623 2024-05-09 07:06:45.000000 qtealeaves-1.1.5/qtealeaves/emulator/abstract_tn.py
+-rw-r--r--   0 quantum    (128) quantum    (128)    13132 2024-04-19 13:19:04.000000 qtealeaves-1.1.5/qtealeaves/emulator/attn_simulator.py
+-rw-r--r--   0 quantum    (128) quantum    (128)     9504 2024-04-19 13:19:04.000000 qtealeaves-1.1.5/qtealeaves/emulator/ed_simulation.py
+-rw-r--r--   0 quantum    (128) quantum    (128)    42393 2024-05-10 14:53:16.000000 qtealeaves-1.1.5/qtealeaves/emulator/lptn_simulator.py
+-rw-r--r--   0 quantum    (128) quantum    (128)    22203 2024-05-09 07:06:45.000000 qtealeaves-1.1.5/qtealeaves/emulator/mpi_mps_simulator.py
+-rw-r--r--   0 quantum    (128) quantum    (128)   111015 2024-05-09 07:06:45.000000 qtealeaves-1.1.5/qtealeaves/emulator/mps_simulator.py
+-rw-r--r--   0 quantum    (128) quantum    (128)    19742 2024-04-19 13:19:04.000000 qtealeaves-1.1.5/qtealeaves/emulator/state_simulator.py
+-rw-r--r--   0 quantum    (128) quantum    (128)    39521 2024-05-10 14:53:16.000000 qtealeaves-1.1.5/qtealeaves/emulator/tn_simulation.py
+-rw-r--r--   0 quantum    (128) quantum    (128)     2535 2024-04-19 13:19:04.000000 qtealeaves-1.1.5/qtealeaves/emulator/tnnode.py
+-rw-r--r--   0 quantum    (128) quantum    (128)   168938 2024-05-08 11:06:39.000000 qtealeaves-1.1.5/qtealeaves/emulator/ttn_simulator.py
+-rw-r--r--   0 quantum    (128) quantum    (128)    46324 2024-05-10 14:53:16.000000 qtealeaves-1.1.5/qtealeaves/emulator/tto_simulator.py
+-rw-r--r--   0 quantum    (128) quantum    (128)     2125 2024-04-19 13:19:04.000000 qtealeaves-1.1.5/qtealeaves/emulator/unitariesprojmeas.py
+drwxr-xr-x   0 quantum    (128) quantum    (128)        0 2024-05-10 15:06:52.991487 qtealeaves-1.1.5/qtealeaves/modeling/
+-rw-r--r--   0 quantum    (128) quantum    (128)     1289 2024-04-19 13:19:04.000000 qtealeaves-1.1.5/qtealeaves/modeling/__init__.py
+-rw-r--r--   0 quantum    (128) quantum    (128)     6956 2024-04-19 13:19:04.000000 qtealeaves-1.1.5/qtealeaves/modeling/baseterm.py
+-rw-r--r--   0 quantum    (128) quantum    (128)     7625 2024-04-19 13:19:04.000000 qtealeaves-1.1.5/qtealeaves/modeling/blockterm2d.py
+-rw-r--r--   0 quantum    (128) quantum    (128)    16787 2024-04-19 13:19:04.000000 qtealeaves-1.1.5/qtealeaves/modeling/localterm.py
+-rw-r--r--   0 quantum    (128) quantum    (128)     7379 2024-04-19 13:19:04.000000 qtealeaves-1.1.5/qtealeaves/modeling/plaquetteterm2d.py
+-rw-r--r--   0 quantum    (128) quantum    (128)    32850 2024-04-19 13:19:04.000000 qtealeaves-1.1.5/qtealeaves/modeling/quantummodel.py
+-rw-r--r--   0 quantum    (128) quantum    (128)     5632 2024-02-26 14:55:43.000000 qtealeaves-1.1.5/qtealeaves/modeling/stringterm1d.py
+-rw-r--r--   0 quantum    (128) quantum    (128)    13220 2024-05-09 07:06:45.000000 qtealeaves-1.1.5/qtealeaves/modeling/twobodyterm1d.py
+-rw-r--r--   0 quantum    (128) quantum    (128)    13088 2024-04-19 13:19:04.000000 qtealeaves-1.1.5/qtealeaves/modeling/twobodyterm2d.py
+-rw-r--r--   0 quantum    (128) quantum    (128)    10657 2024-04-19 13:19:04.000000 qtealeaves-1.1.5/qtealeaves/modeling/twobodyterm3d.py
+drwxr-xr-x   0 quantum    (128) quantum    (128)        0 2024-05-10 15:06:52.991487 qtealeaves-1.1.5/qtealeaves/models/
+-rw-r--r--   0 quantum    (128) quantum    (128)      766 2022-11-30 17:54:07.000000 qtealeaves-1.1.5/qtealeaves/models/__init__.py
+-rw-r--r--   0 quantum    (128) quantum    (128)     2720 2022-11-30 17:54:07.000000 qtealeaves-1.1.5/qtealeaves/models/bosehubbard.py
+-rw-r--r--   0 quantum    (128) quantum    (128)     4682 2023-10-26 07:55:27.000000 qtealeaves-1.1.5/qtealeaves/models/quantumising.py
+-rw-r--r--   0 quantum    (128) quantum    (128)     1736 2022-11-30 17:54:07.000000 qtealeaves-1.1.5/qtealeaves/models/xxzmodel.py
+drwxr-xr-x   0 quantum    (128) quantum    (128)        0 2024-05-10 15:06:52.991487 qtealeaves-1.1.5/qtealeaves/mpos/
+-rw-r--r--   0 quantum    (128) quantum    (128)     1239 2024-04-19 13:19:04.000000 qtealeaves-1.1.5/qtealeaves/mpos/__init__.py
+-rw-r--r--   0 quantum    (128) quantum    (128)     4018 2024-04-19 13:19:04.000000 qtealeaves-1.1.5/qtealeaves/mpos/abstracteffop.py
+-rw-r--r--   0 quantum    (128) quantum    (128)    15982 2024-04-19 13:19:04.000000 qtealeaves-1.1.5/qtealeaves/mpos/densempos.py
+-rw-r--r--   0 quantum    (128) quantum    (128)    15908 2024-04-19 13:19:04.000000 qtealeaves-1.1.5/qtealeaves/mpos/disentangler.py
+-rw-r--r--   0 quantum    (128) quantum    (128)    76751 2024-04-19 13:19:04.000000 qtealeaves-1.1.5/qtealeaves/mpos/indexedtpo.py
+-rw-r--r--   0 quantum    (128) quantum    (128)    23290 2024-04-19 13:19:04.000000 qtealeaves-1.1.5/qtealeaves/mpos/sparsematrixoperator.py
+-rw-r--r--   0 quantum    (128) quantum    (128)    20242 2024-04-19 13:19:04.000000 qtealeaves-1.1.5/qtealeaves/mpos/sparsematrixproductoperator.py
+-rw-r--r--   0 quantum    (128) quantum    (128)    21798 2024-04-19 13:19:04.000000 qtealeaves-1.1.5/qtealeaves/mpos/tensorproductoperator.py
+drwxr-xr-x   0 quantum    (128) quantum    (128)        0 2024-05-10 15:06:52.991487 qtealeaves-1.1.5/qtealeaves/observables/
+-rw-r--r--   0 quantum    (128) quantum    (128)     1530 2024-01-12 22:24:30.000000 qtealeaves-1.1.5/qtealeaves/observables/__init__.py
+-rw-r--r--   0 quantum    (128) quantum    (128)     6009 2024-04-19 13:19:04.000000 qtealeaves-1.1.5/qtealeaves/observables/bond_entropy.py
+-rw-r--r--   0 quantum    (128) quantum    (128)    19724 2024-04-19 13:19:04.000000 qtealeaves-1.1.5/qtealeaves/observables/correlation.py
+-rw-r--r--   0 quantum    (128) quantum    (128)    12681 2024-04-19 13:19:04.000000 qtealeaves-1.1.5/qtealeaves/observables/custom_correlation.py
+-rw-r--r--   0 quantum    (128) quantum    (128)     4703 2024-04-19 13:19:04.000000 qtealeaves-1.1.5/qtealeaves/observables/distance2pure.py
+-rw-r--r--   0 quantum    (128) quantum    (128)     5908 2024-04-19 13:19:04.000000 qtealeaves-1.1.5/qtealeaves/observables/local.py
+-rw-r--r--   0 quantum    (128) quantum    (128)     7874 2024-04-19 13:19:04.000000 qtealeaves-1.1.5/qtealeaves/observables/probabilities.py
+-rw-r--r--   0 quantum    (128) quantum    (128)     5653 2024-04-19 13:19:04.000000 qtealeaves-1.1.5/qtealeaves/observables/projective.py
+-rw-r--r--   0 quantum    (128) quantum    (128)     5110 2024-04-19 13:19:04.000000 qtealeaves-1.1.5/qtealeaves/observables/state2file.py
+-rw-r--r--   0 quantum    (128) quantum    (128)     5834 2024-04-19 13:19:04.000000 qtealeaves-1.1.5/qtealeaves/observables/tensor_product.py
+-rw-r--r--   0 quantum    (128) quantum    (128)     5609 2024-04-19 13:19:04.000000 qtealeaves-1.1.5/qtealeaves/observables/timecorrelator.py
+-rw-r--r--   0 quantum    (128) quantum    (128)     6351 2024-04-19 13:19:04.000000 qtealeaves-1.1.5/qtealeaves/observables/tnobase.py
+-rw-r--r--   0 quantum    (128) quantum    (128)    18721 2024-04-19 13:19:04.000000 qtealeaves-1.1.5/qtealeaves/observables/tnobservables.py
+-rw-r--r--   0 quantum    (128) quantum    (128)    10161 2024-04-19 13:19:04.000000 qtealeaves-1.1.5/qtealeaves/observables/weighted_sum.py
+drwxr-xr-x   0 quantum    (128) quantum    (128)        0 2024-05-10 15:06:52.991487 qtealeaves-1.1.5/qtealeaves/operators/
+-rw-r--r--   0 quantum    (128) quantum    (128)     1004 2023-10-26 07:55:27.000000 qtealeaves-1.1.5/qtealeaves/operators/__init__.py
+-rw-r--r--   0 quantum    (128) quantum    (128)     2894 2024-04-19 13:19:04.000000 qtealeaves-1.1.5/qtealeaves/operators/bosonicoperators.py
+-rw-r--r--   0 quantum    (128) quantum    (128)     2620 2024-05-02 13:16:14.000000 qtealeaves-1.1.5/qtealeaves/operators/combinedoperators.py
+-rw-r--r--   0 quantum    (128) quantum    (128)     4143 2022-11-30 17:54:07.000000 qtealeaves-1.1.5/qtealeaves/operators/quditoperators.py
+-rw-r--r--   0 quantum    (128) quantum    (128)     1368 2024-04-19 13:19:04.000000 qtealeaves-1.1.5/qtealeaves/operators/spinoperators.py
+-rw-r--r--   0 quantum    (128) quantum    (128)     9216 2024-04-19 13:19:04.000000 qtealeaves-1.1.5/qtealeaves/operators/tnoperators.py
+-rw-r--r--   0 quantum    (128) quantum    (128)    68904 2024-04-19 13:19:04.000000 qtealeaves-1.1.5/qtealeaves/simulation_setup.py
+drwxr-xr-x   0 quantum    (128) quantum    (128)        0 2024-05-10 15:06:52.991487 qtealeaves-1.1.5/qtealeaves/solvers/
+-rw-r--r--   0 quantum    (128) quantum    (128)      698 2024-04-19 13:19:04.000000 qtealeaves-1.1.5/qtealeaves/solvers/__init__.py
+-rw-r--r--   0 quantum    (128) quantum    (128)     4067 2024-04-19 13:19:04.000000 qtealeaves-1.1.5/qtealeaves/solvers/eigen_solver.py
+-rw-r--r--   0 quantum    (128) quantum    (128)     7352 2024-05-10 14:53:16.000000 qtealeaves-1.1.5/qtealeaves/solvers/krylovexp_solver.py
+drwxr-xr-x   0 quantum    (128) quantum    (128)        0 2024-05-10 15:06:52.991487 qtealeaves-1.1.5/qtealeaves/tensors/
+-rw-r--r--   0 quantum    (128) quantum    (128)      801 2024-04-19 13:19:04.000000 qtealeaves-1.1.5/qtealeaves/tensors/__init__.py
+-rw-r--r--   0 quantum    (128) quantum    (128)    17043 2024-04-19 13:19:04.000000 qtealeaves-1.1.5/qtealeaves/tensors/abstracttensor.py
+-rw-r--r--   0 quantum    (128) quantum    (128)    75600 2024-05-09 07:06:45.000000 qtealeaves-1.1.5/qtealeaves/tensors/tensor.py
+-rw-r--r--   0 quantum    (128) quantum    (128)     1663 2024-04-19 13:19:04.000000 qtealeaves-1.1.5/qtealeaves/tensors/tensor_backend.py
+drwxr-xr-x   0 quantum    (128) quantum    (128)        0 2024-05-10 15:06:52.995487 qtealeaves-1.1.5/qtealeaves/tooling/
+-rw-r--r--   0 quantum    (128) quantum    (128)     1179 2024-04-19 13:19:04.000000 qtealeaves-1.1.5/qtealeaves/tooling/__init__.py
+-rw-r--r--   0 quantum    (128) quantum    (128)    17831 2024-04-19 13:19:04.000000 qtealeaves-1.1.5/qtealeaves/tooling/fortran_interfaces.py
+-rw-r--r--   0 quantum    (128) quantum    (128)    47759 2024-04-19 13:19:04.000000 qtealeaves-1.1.5/qtealeaves/tooling/hilbert_curvature.py
+-rw-r--r--   0 quantum    (128) quantum    (128)     5883 2024-04-19 13:19:04.000000 qtealeaves-1.1.5/qtealeaves/tooling/lattice_layout.py
+-rw-r--r--   0 quantum    (128) quantum    (128)     4080 2024-04-19 13:19:04.000000 qtealeaves-1.1.5/qtealeaves/tooling/parameterized.py
+-rw-r--r--   0 quantum    (128) quantum    (128)     1768 2024-04-19 13:19:04.000000 qtealeaves-1.1.5/qtealeaves/tooling/permutations.py
+-rw-r--r--   0 quantum    (128) quantum    (128)     1785 2024-04-19 13:19:04.000000 qtealeaves-1.1.5/qtealeaves/tooling/restrictedclasses.py
+-rw-r--r--   0 quantum    (128) quantum    (128)      531 2024-05-10 14:53:16.000000 qtealeaves-1.1.5/qtealeaves/version.py
+drwxr-xr-x   0 quantum    (128) quantum    (128)        0 2024-05-10 15:06:52.995487 qtealeaves-1.1.5/qtealeaves.egg-info/
+-rw-r--r--   0 quantum    (128) quantum    (128)     3319 2024-05-10 15:06:52.000000 qtealeaves-1.1.5/qtealeaves.egg-info/PKG-INFO
+-rw-r--r--   0 quantum    (128) quantum    (128)     3297 2024-05-10 15:06:52.000000 qtealeaves-1.1.5/qtealeaves.egg-info/SOURCES.txt
+-rw-r--r--   0 quantum    (128) quantum    (128)        1 2024-05-10 15:06:52.000000 qtealeaves-1.1.5/qtealeaves.egg-info/dependency_links.txt
+-rw-r--r--   0 quantum    (128) quantum    (128)       42 2024-05-10 15:06:52.000000 qtealeaves-1.1.5/qtealeaves.egg-info/requires.txt
+-rw-r--r--   0 quantum    (128) quantum    (128)       11 2024-05-10 15:06:52.000000 qtealeaves-1.1.5/qtealeaves.egg-info/top_level.txt
+-rw-r--r--   0 quantum    (128) quantum    (128)       38 2024-05-10 15:06:52.995487 qtealeaves-1.1.5/setup.cfg
+-rw-r--r--   0 quantum    (128) quantum    (128)     3041 2024-05-02 13:16:14.000000 qtealeaves-1.1.5/setup.py
+drwxr-xr-x   0 quantum    (128) quantum    (128)        0 2024-05-10 15:06:52.995487 qtealeaves-1.1.5/tests/
+-rw-r--r--   0 quantum    (128) quantum    (128)     1332 2022-11-30 17:54:07.000000 qtealeaves-1.1.5/tests/tests_formatting.py
+-rw-r--r--   0 quantum    (128) quantum    (128)     1504 2023-10-26 07:55:27.000000 qtealeaves-1.1.5/tests/tests_fortran_interface.py
+-rw-r--r--   0 quantum    (128) quantum    (128)     9308 2024-05-09 07:06:45.000000 qtealeaves-1.1.5/tests/tests_hilbert_curvature.py
+-rw-r--r--   0 quantum    (128) quantum    (128)     2732 2024-04-19 13:19:04.000000 qtealeaves-1.1.5/tests/tests_lattice_layout.py
+-rw-r--r--   0 quantum    (128) quantum    (128)    27539 2024-04-19 13:19:04.000000 qtealeaves-1.1.5/tests/tests_linter.py
+-rw-r--r--   0 quantum    (128) quantum    (128)     5818 2023-10-26 07:55:27.000000 qtealeaves-1.1.5/tests/tests_model_terms.py
+-rw-r--r--   0 quantum    (128) quantum    (128)     9812 2024-04-19 13:19:04.000000 qtealeaves-1.1.5/tests/tests_observables.py
+-rw-r--r--   0 quantum    (128) quantum    (128)     1858 2023-01-26 15:54:33.000000 qtealeaves-1.1.5/tests/tests_operators.py
+-rw-r--r--   0 quantum    (128) quantum    (128)     2962 2024-04-19 13:19:04.000000 qtealeaves-1.1.5/tests/tests_quantum_trajectories.py
+-rw-r--r--   0 quantum    (128) quantum    (128)     2553 2022-11-30 17:54:07.000000 qtealeaves-1.1.5/tests/tests_rydberg_model.py
+-rw-r--r--   0 quantum    (128) quantum    (128)     4401 2024-04-19 13:19:04.000000 qtealeaves-1.1.5/tests/tests_simulation_setup.py
+-rw-r--r--   0 quantum    (128) quantum    (128)    14206 2024-05-09 07:06:45.000000 qtealeaves-1.1.5/tests/tests_tn_simulation.py
```

### Comparing `qtealeaves-1.1.4/LICENSE` & `qtealeaves-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `qtealeaves-1.1.4/PKG-INFO` & `qtealeaves-1.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qtealeaves
-Version: 1.1.4
+Version: 1.1.5
 Summary: Quantum TEA's python tensor network library
 Home-page: https://baltig.infn.it/quantum_tea_leaves/py_api_quantum_tea_leaves.git
 Author: Marco Ballarin, Giovanni Cataldi, Aurora Costantini, Daniel Jaschke, Giuseppe Magnifico, Simone Notarnicola, Alice Pagano, Luka Pavesic, Davide Rattacaso, Marco Rigobello, Nora Reinić, Simone Scarlatella, Darvin Wanisch
 Author-email: 
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `qtealeaves-1.1.4/README.md` & `qtealeaves-1.1.5/README.md`

 * *Files identical despite different names*

### Comparing `qtealeaves-1.1.4/qtealeaves/__init__.py` & `qtealeaves-1.1.5/qtealeaves/__init__.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-1.1.4/qtealeaves/convergence_parameters/__init__.py` & `qtealeaves-1.1.5/qtealeaves/convergence_parameters/__init__.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-1.1.4/qtealeaves/convergence_parameters/conv_params.py` & `qtealeaves-1.1.5/qtealeaves/convergence_parameters/conv_params.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-1.1.4/qtealeaves/convergence_parameters/conv_params_finite_temp.py` & `qtealeaves-1.1.5/qtealeaves/convergence_parameters/conv_params_finite_temp.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-1.1.4/qtealeaves/emulator/__init__.py` & `qtealeaves-1.1.5/qtealeaves/emulator/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -25,14 +25,20 @@
 
 from . import mpi_mps_simulator
 from .mpi_mps_simulator import *
 
 from . import ttn_simulator
 from .ttn_simulator import *
 
+from . import lptn_simulator
+from .lptn_simulator import *
+
+from . import tto_simulator
+from .tto_simulator import *
+
 from . import attn_simulator
 from .attn_simulator import *
 
 from . import state_simulator
 from .state_simulator import *
 
 from . import ed_simulation
@@ -44,11 +50,13 @@
 
 __all__ = tnnode.__all__.copy()
 __all__ += unitariesprojmeas.__all__.copy()
 __all__ += abstract_tn.__all__.copy()
 __all__ += mps_simulator.__all__.copy()
 __all__ += mpi_mps_simulator.__all__.copy()
 __all__ += ttn_simulator.__all__.copy()
+__all__ += lptn_simulator.__all__.copy()
+__all__ += tto_simulator.__all__.copy()
 __all__ += attn_simulator.__all__.copy()
 __all__ += state_simulator.__all__.copy()
 __all__ += ed_simulation.__all__.copy()
 __all__ += tn_simulation.__all__.copy()
```

### Comparing `qtealeaves-1.1.4/qtealeaves/emulator/abstract_tn.py` & `qtealeaves-1.1.5/qtealeaves/emulator/abstract_tn.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-1.1.4/qtealeaves/emulator/attn_simulator.py` & `qtealeaves-1.1.5/qtealeaves/emulator/attn_simulator.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-1.1.4/qtealeaves/emulator/ed_simulation.py` & `qtealeaves-1.1.5/qtealeaves/emulator/ed_simulation.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-1.1.4/qtealeaves/emulator/lptn_simulator.py` & `qtealeaves-1.1.5/qtealeaves/emulator/lptn_simulator.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,14 +24,16 @@
 import numpy as np
 import numpy.linalg as nla
 from qtealeaves.convergence_parameters import TNConvergenceParameters
 from qtealeaves.tensors import _AbstractQteaTensor
 from .abstract_tn import _AbstractTN
 from .mps_simulator import MPS
 
+__all__ = ["LPTN"]
+
 
 class LPTN(_AbstractTN):
     """
     LOCALLY PURIFIED TENSOR NETWORK CLASS - operator
     order of legs: 0 - left bond, 1 - lower (physical) leg,
     2 - upper leg, 3 - right bond
```

### Comparing `qtealeaves-1.1.4/qtealeaves/emulator/mpi_mps_simulator.py` & `qtealeaves-1.1.5/qtealeaves/emulator/mpi_mps_simulator.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-1.1.4/qtealeaves/emulator/mps_simulator.py` & `qtealeaves-1.1.5/qtealeaves/emulator/mps_simulator.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-1.1.4/qtealeaves/emulator/state_simulator.py` & `qtealeaves-1.1.5/qtealeaves/emulator/state_simulator.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-1.1.4/qtealeaves/emulator/tn_simulation.py` & `qtealeaves-1.1.5/qtealeaves/emulator/tn_simulation.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 # that they have been altered from the originals.
 
 """
 The module contains a light-weight execution of a tensor network simulations for:
 
 - MPS
 - TTN
+- aTTN (only correlation measurements)
 
 """
 
 # pylint: disable=too-many-locals
 # pylint: disable=too-many-lines
 # pylint: disable=too-many-arguments
 # pylint: disable=too-many-branches
```

### Comparing `qtealeaves-1.1.4/qtealeaves/emulator/tnnode.py` & `qtealeaves-1.1.5/qtealeaves/emulator/tnnode.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-1.1.4/qtealeaves/emulator/ttn_simulator.py` & `qtealeaves-1.1.5/qtealeaves/emulator/ttn_simulator.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-1.1.4/qtealeaves/emulator/tto_simulator.py` & `qtealeaves-1.1.5/qtealeaves/emulator/tto_simulator.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,14 +18,16 @@
 import scipy.optimize as scop
 import numpy as np
 import numpy.linalg as nla
 from qtealeaves.emulator.lptn_simulator import LPTN
 from qtealeaves.convergence_parameters import TNConvergenceParameters
 from .ttn_simulator import TTN, TTNLayer
 
+__all__ = ["TTO"]
+
 
 class TTO(TTN):
     r"""
     TREE TENSOR OPERATOR - represents a density matrix
 
     Parameters
     ----------
```

### Comparing `qtealeaves-1.1.4/qtealeaves/emulator/unitariesprojmeas.py` & `qtealeaves-1.1.5/qtealeaves/emulator/unitariesprojmeas.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-1.1.4/qtealeaves/modeling/__init__.py` & `qtealeaves-1.1.5/qtealeaves/modeling/__init__.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-1.1.4/qtealeaves/modeling/baseterm.py` & `qtealeaves-1.1.5/qtealeaves/modeling/baseterm.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-1.1.4/qtealeaves/modeling/blockterm2d.py` & `qtealeaves-1.1.5/qtealeaves/modeling/blockterm2d.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-1.1.4/qtealeaves/modeling/localterm.py` & `qtealeaves-1.1.5/qtealeaves/modeling/localterm.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-1.1.4/qtealeaves/modeling/plaquetteterm2d.py` & `qtealeaves-1.1.5/qtealeaves/modeling/plaquetteterm2d.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-1.1.4/qtealeaves/modeling/quantummodel.py` & `qtealeaves-1.1.5/qtealeaves/modeling/quantummodel.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-1.1.4/qtealeaves/modeling/stringterm1d.py` & `qtealeaves-1.1.5/qtealeaves/modeling/stringterm1d.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-1.1.4/qtealeaves/modeling/twobodyterm1d.py` & `qtealeaves-1.1.5/qtealeaves/modeling/twobodyterm1d.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-1.1.4/qtealeaves/modeling/twobodyterm2d.py` & `qtealeaves-1.1.5/qtealeaves/modeling/twobodyterm2d.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-1.1.4/qtealeaves/modeling/twobodyterm3d.py` & `qtealeaves-1.1.5/qtealeaves/modeling/twobodyterm3d.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-1.1.4/qtealeaves/models/__init__.py` & `qtealeaves-1.1.5/qtealeaves/models/__init__.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-1.1.4/qtealeaves/models/bosehubbard.py` & `qtealeaves-1.1.5/qtealeaves/models/bosehubbard.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-1.1.4/qtealeaves/models/quantumising.py` & `qtealeaves-1.1.5/qtealeaves/models/quantumising.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-1.1.4/qtealeaves/models/xxzmodel.py` & `qtealeaves-1.1.5/qtealeaves/models/xxzmodel.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-1.1.4/qtealeaves/mpos/__init__.py` & `qtealeaves-1.1.5/qtealeaves/mpos/__init__.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-1.1.4/qtealeaves/mpos/abstracteffop.py` & `qtealeaves-1.1.5/qtealeaves/mpos/abstracteffop.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-1.1.4/qtealeaves/mpos/densempos.py` & `qtealeaves-1.1.5/qtealeaves/mpos/densempos.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-1.1.4/qtealeaves/mpos/disentangler.py` & `qtealeaves-1.1.5/qtealeaves/mpos/disentangler.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-1.1.4/qtealeaves/mpos/indexedtpo.py` & `qtealeaves-1.1.5/qtealeaves/mpos/indexedtpo.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-1.1.4/qtealeaves/mpos/sparsematrixoperator.py` & `qtealeaves-1.1.5/qtealeaves/mpos/sparsematrixoperator.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-1.1.4/qtealeaves/mpos/sparsematrixproductoperator.py` & `qtealeaves-1.1.5/qtealeaves/mpos/sparsematrixproductoperator.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-1.1.4/qtealeaves/mpos/tensorproductoperator.py` & `qtealeaves-1.1.5/qtealeaves/mpos/tensorproductoperator.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-1.1.4/qtealeaves/observables/__init__.py` & `qtealeaves-1.1.5/qtealeaves/observables/__init__.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-1.1.4/qtealeaves/observables/bond_entropy.py` & `qtealeaves-1.1.5/qtealeaves/observables/bond_entropy.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-1.1.4/qtealeaves/observables/correlation.py` & `qtealeaves-1.1.5/qtealeaves/observables/correlation.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-1.1.4/qtealeaves/observables/custom_correlation.py` & `qtealeaves-1.1.5/qtealeaves/observables/custom_correlation.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-1.1.4/qtealeaves/observables/distance2pure.py` & `qtealeaves-1.1.5/qtealeaves/observables/distance2pure.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-1.1.4/qtealeaves/observables/local.py` & `qtealeaves-1.1.5/qtealeaves/observables/local.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-1.1.4/qtealeaves/observables/probabilities.py` & `qtealeaves-1.1.5/qtealeaves/observables/probabilities.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-1.1.4/qtealeaves/observables/projective.py` & `qtealeaves-1.1.5/qtealeaves/observables/projective.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-1.1.4/qtealeaves/observables/state2file.py` & `qtealeaves-1.1.5/qtealeaves/observables/state2file.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-1.1.4/qtealeaves/observables/tensor_product.py` & `qtealeaves-1.1.5/qtealeaves/observables/tensor_product.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-1.1.4/qtealeaves/observables/timecorrelator.py` & `qtealeaves-1.1.5/qtealeaves/observables/timecorrelator.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-1.1.4/qtealeaves/observables/tnobase.py` & `qtealeaves-1.1.5/qtealeaves/observables/tnobase.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-1.1.4/qtealeaves/observables/tnobservables.py` & `qtealeaves-1.1.5/qtealeaves/observables/tnobservables.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-1.1.4/qtealeaves/observables/weighted_sum.py` & `qtealeaves-1.1.5/qtealeaves/observables/weighted_sum.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-1.1.4/qtealeaves/operators/__init__.py` & `qtealeaves-1.1.5/qtealeaves/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-1.1.4/qtealeaves/operators/bosonicoperators.py` & `qtealeaves-1.1.5/qtealeaves/operators/bosonicoperators.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-1.1.4/qtealeaves/operators/combinedoperators.py` & `qtealeaves-1.1.5/qtealeaves/operators/combinedoperators.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-1.1.4/qtealeaves/operators/quditoperators.py` & `qtealeaves-1.1.5/qtealeaves/operators/quditoperators.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-1.1.4/qtealeaves/operators/spinoperators.py` & `qtealeaves-1.1.5/qtealeaves/operators/spinoperators.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-1.1.4/qtealeaves/operators/tnoperators.py` & `qtealeaves-1.1.5/qtealeaves/operators/tnoperators.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-1.1.4/qtealeaves/simulation_setup.py` & `qtealeaves-1.1.5/qtealeaves/simulation_setup.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-1.1.4/qtealeaves/solvers/__init__.py` & `qtealeaves-1.1.5/qtealeaves/solvers/__init__.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-1.1.4/qtealeaves/solvers/eigen_solver.py` & `qtealeaves-1.1.5/qtealeaves/solvers/eigen_solver.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-1.1.4/qtealeaves/solvers/krylovexp_solver.py` & `qtealeaves-1.1.5/qtealeaves/solvers/krylovexp_solver.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # of this source tree or at http://www.apache.org/licenses/LICENSE-2.0.
 #
 # Any modifications or derivative works of this code must retain this
 # copyright notice, and modified files need to carry a notice indicating
 # that they have been altered from the originals.
 
 """
-The module contains solvers for the Krylov expoential as an API (multiplication
+The module contains solvers for the Krylov exponetial as an API (multiplication
 matrix-vector are passed as function, vector class needs only a few attributes).
 
 **Attributes needed for vector class**
 
 * `norm`
 * `dot` for inner product between two vectors.
 * `add_update(self, other, factor_self, factor_other)
```

### Comparing `qtealeaves-1.1.4/qtealeaves/tensors/__init__.py` & `qtealeaves-1.1.5/qtealeaves/tensors/__init__.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-1.1.4/qtealeaves/tensors/abstracttensor.py` & `qtealeaves-1.1.5/qtealeaves/tensors/abstracttensor.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-1.1.4/qtealeaves/tensors/tensor.py` & `qtealeaves-1.1.5/qtealeaves/tensors/tensor.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-1.1.4/qtealeaves/tensors/tensor_backend.py` & `qtealeaves-1.1.5/qtealeaves/tensors/tensor_backend.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-1.1.4/qtealeaves/tooling/__init__.py` & `qtealeaves-1.1.5/qtealeaves/tooling/__init__.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-1.1.4/qtealeaves/tooling/fortran_interfaces.py` & `qtealeaves-1.1.5/qtealeaves/tooling/fortran_interfaces.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-1.1.4/qtealeaves/tooling/hilbert_curvature.py` & `qtealeaves-1.1.5/qtealeaves/tooling/hilbert_curvature.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-1.1.4/qtealeaves/tooling/lattice_layout.py` & `qtealeaves-1.1.5/qtealeaves/tooling/lattice_layout.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-1.1.4/qtealeaves/tooling/parameterized.py` & `qtealeaves-1.1.5/qtealeaves/tooling/parameterized.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-1.1.4/qtealeaves/tooling/permutations.py` & `qtealeaves-1.1.5/qtealeaves/tooling/permutations.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-1.1.4/qtealeaves/tooling/restrictedclasses.py` & `qtealeaves-1.1.5/qtealeaves/tooling/restrictedclasses.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-1.1.4/qtealeaves/version.py` & `qtealeaves-1.1.5/qtealeaves/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 # Any modifications or derivative works of this code must retain this
 # copyright notice, and modified files need to carry a notice indicating
 # that they have been altered from the originals.
 
 """
 Version string, e.g., for installation script.
 """
-__version__ = "1.1.4"
+__version__ = "1.1.5"
```

### Comparing `qtealeaves-1.1.4/qtealeaves.egg-info/PKG-INFO` & `qtealeaves-1.1.5/qtealeaves.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qtealeaves
-Version: 1.1.4
+Version: 1.1.5
 Summary: Quantum TEA's python tensor network library
 Home-page: https://baltig.infn.it/quantum_tea_leaves/py_api_quantum_tea_leaves.git
 Author: Marco Ballarin, Giovanni Cataldi, Aurora Costantini, Daniel Jaschke, Giuseppe Magnifico, Simone Notarnicola, Alice Pagano, Luka Pavesic, Davide Rattacaso, Marco Rigobello, Nora Reinić, Simone Scarlatella, Darvin Wanisch
 Author-email: 
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `qtealeaves-1.1.4/qtealeaves.egg-info/SOURCES.txt` & `qtealeaves-1.1.5/qtealeaves.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `qtealeaves-1.1.4/setup.py` & `qtealeaves-1.1.5/setup.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-1.1.4/tests/tests_formatting.py` & `qtealeaves-1.1.5/tests/tests_formatting.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-1.1.4/tests/tests_fortran_interface.py` & `qtealeaves-1.1.5/tests/tests_fortran_interface.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-1.1.4/tests/tests_hilbert_curvature.py` & `qtealeaves-1.1.5/tests/tests_hilbert_curvature.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-1.1.4/tests/tests_lattice_layout.py` & `qtealeaves-1.1.5/tests/tests_lattice_layout.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-1.1.4/tests/tests_linter.py` & `qtealeaves-1.1.5/tests/tests_linter.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-1.1.4/tests/tests_model_terms.py` & `qtealeaves-1.1.5/tests/tests_model_terms.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-1.1.4/tests/tests_observables.py` & `qtealeaves-1.1.5/tests/tests_observables.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-1.1.4/tests/tests_operators.py` & `qtealeaves-1.1.5/tests/tests_operators.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-1.1.4/tests/tests_quantum_trajectories.py` & `qtealeaves-1.1.5/tests/tests_quantum_trajectories.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-1.1.4/tests/tests_rydberg_model.py` & `qtealeaves-1.1.5/tests/tests_rydberg_model.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-1.1.4/tests/tests_simulation_setup.py` & `qtealeaves-1.1.5/tests/tests_simulation_setup.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-1.1.4/tests/tests_tn_simulation.py` & `qtealeaves-1.1.5/tests/tests_tn_simulation.py`

 * *Files identical despite different names*

