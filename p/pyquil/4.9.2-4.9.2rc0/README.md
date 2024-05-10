# Comparing `tmp/pyquil-4.9.2.tar.gz` & `tmp/pyquil-4.9.2rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyquil-4.9.2.tar", max compression
+gzip compressed data, was "pyquil-4.9.2rc0.tar", max compression
```

## Comparing `pyquil-4.9.2.tar` & `pyquil-4.9.2rc0.tar`

### file list

```diff
@@ -1,67 +1,67 @@
--rw-r--r--   0        0        0    11358 2024-04-17 21:33:12.559846 pyquil-4.9.2/LICENSE
--rw-r--r--   0        0        0     1779 2024-04-17 21:33:12.559846 pyquil-4.9.2/NOTICE.md
--rw-r--r--   0        0        0     8944 2024-04-17 21:33:12.559846 pyquil-4.9.2/README.md
--rw-r--r--   0        0        0     2776 2024-04-17 21:33:12.795846 pyquil-4.9.2/pyproject.toml
--rw-r--r--   0        0        0      159 2024-04-17 21:33:12.795846 pyquil-4.9.2/pyquil/__init__.py
--rw-r--r--   0        0        0     1082 2024-04-17 21:33:12.795846 pyquil-4.9.2/pyquil/_version.py
--rw-r--r--   0        0        0     2129 2024-04-17 21:33:12.795846 pyquil-4.9.2/pyquil/api/__init__.py
--rw-r--r--   0        0        0     8884 2024-04-17 21:33:12.795846 pyquil-4.9.2/pyquil/api/_abstract_compiler.py
--rw-r--r--   0        0        0     7377 2024-04-17 21:33:12.795846 pyquil-4.9.2/pyquil/api/_benchmark.py
--rw-r--r--   0        0        0     9942 2024-04-17 21:33:12.795846 pyquil-4.9.2/pyquil/api/_compiler.py
--rw-r--r--   0        0        0     5554 2024-04-17 21:33:12.795846 pyquil-4.9.2/pyquil/api/_compiler_client.py
--rw-r--r--   0        0        0     4265 2024-04-17 21:33:12.795846 pyquil-4.9.2/pyquil/api/_errors.py
--rw-r--r--   0        0        0     1010 2024-04-17 21:33:12.795846 pyquil-4.9.2/pyquil/api/_logger.py
--rw-r--r--   0        0        0     7568 2024-04-17 21:33:12.795846 pyquil-4.9.2/pyquil/api/_qam.py
--rw-r--r--   0        0        0    11336 2024-04-17 21:33:12.795846 pyquil-4.9.2/pyquil/api/_qpu.py
--rw-r--r--   0        0        0    55258 2024-04-17 21:33:12.795846 pyquil-4.9.2/pyquil/api/_quantum_computer.py
--rw-r--r--   0        0        0     8637 2024-04-17 21:33:12.795846 pyquil-4.9.2/pyquil/api/_qvm.py
--rw-r--r--   0        0        0     5562 2024-04-17 21:33:12.795846 pyquil-4.9.2/pyquil/api/_rewrite_arithmetic.py
--rw-r--r--   0        0        0    10749 2024-04-17 21:33:12.795846 pyquil-4.9.2/pyquil/api/_wavefunction_simulator.py
--rw-r--r--   0        0        0      369 2024-04-17 21:33:12.795846 pyquil-4.9.2/pyquil/diagnostics.py
--rw-r--r--   0        0        0     1371 2024-04-17 21:33:12.795846 pyquil-4.9.2/pyquil/experiment/__init__.py
--rw-r--r--   0        0        0      896 2024-04-17 21:33:12.795846 pyquil-4.9.2/pyquil/experiment/_calibration.py
--rw-r--r--   0        0        0    15705 2024-04-17 21:33:12.799846 pyquil-4.9.2/pyquil/experiment/_group.py
--rw-r--r--   0        0        0    22783 2024-04-17 21:33:12.799846 pyquil-4.9.2/pyquil/experiment/_main.py
--rw-r--r--   0        0        0     8213 2024-04-17 21:33:12.799846 pyquil-4.9.2/pyquil/experiment/_memory.py
--rw-r--r--   0        0        0     5547 2024-04-17 21:33:12.799846 pyquil-4.9.2/pyquil/experiment/_program.py
--rw-r--r--   0        0        0     9047 2024-04-17 21:33:12.799846 pyquil-4.9.2/pyquil/experiment/_result.py
--rw-r--r--   0        0        0     7469 2024-04-17 21:33:12.799846 pyquil-4.9.2/pyquil/experiment/_setting.py
--rw-r--r--   0        0        0      934 2024-04-17 21:33:12.799846 pyquil-4.9.2/pyquil/experiment/_symmetrization.py
--rw-r--r--   0        0        0      282 2024-04-17 21:33:12.799846 pyquil-4.9.2/pyquil/external/README.md
--rw-r--r--   0        0        0        0 2024-04-17 21:33:12.799846 pyquil-4.9.2/pyquil/external/__init__.py
--rw-r--r--   0        0        0     9858 2024-04-17 21:33:12.799846 pyquil-4.9.2/pyquil/external/rpcq.py
--rw-r--r--   0        0        0    42387 2024-04-17 21:33:12.799846 pyquil-4.9.2/pyquil/gates.py
--rw-r--r--   0        0        0      201 2024-04-17 21:33:12.799846 pyquil-4.9.2/pyquil/latex/__init__.py
--rw-r--r--   0        0        0    18720 2024-04-17 21:33:12.799846 pyquil-4.9.2/pyquil/latex/_diagram.py
--rw-r--r--   0        0        0     3452 2024-04-17 21:33:12.799846 pyquil-4.9.2/pyquil/latex/_ipython.py
--rw-r--r--   0        0        0     4041 2024-04-17 21:33:12.799846 pyquil-4.9.2/pyquil/latex/_main.py
--rw-r--r--   0        0        0     1266 2024-04-17 21:33:12.799846 pyquil-4.9.2/pyquil/latex/latex_generation.py
--rw-r--r--   0        0        0    31958 2024-04-17 21:33:12.799846 pyquil-4.9.2/pyquil/noise.py
--rw-r--r--   0        0        0     3346 2024-04-17 21:33:12.799846 pyquil-4.9.2/pyquil/noise_gates.py
--rw-r--r--   0        0        0    15865 2024-04-17 21:33:12.799846 pyquil-4.9.2/pyquil/operator_estimation.py
--rw-r--r--   0        0        0    42310 2024-04-17 21:33:12.799846 pyquil-4.9.2/pyquil/paulis.py
--rw-r--r--   0        0        0        0 2024-04-17 21:33:12.799846 pyquil-4.9.2/pyquil/py.typed
--rw-r--r--   0        0        0    19676 2024-04-17 21:33:12.799846 pyquil-4.9.2/pyquil/pyqvm.py
--rw-r--r--   0        0        0      336 2024-04-17 21:33:12.799846 pyquil-4.9.2/pyquil/quantum_processor/__init__.py
--rw-r--r--   0        0        0     1662 2024-04-17 21:33:12.799846 pyquil-4.9.2/pyquil/quantum_processor/_base.py
--rw-r--r--   0        0        0        0 2024-04-17 21:33:12.799846 pyquil-4.9.2/pyquil/quantum_processor/_isa.py
--rw-r--r--   0        0        0      774 2024-04-17 21:33:12.799846 pyquil-4.9.2/pyquil/quantum_processor/compiler.py
--rw-r--r--   0        0        0     1856 2024-04-17 21:33:12.799846 pyquil-4.9.2/pyquil/quantum_processor/graph.py
--rw-r--r--   0        0        0     2714 2024-04-17 21:33:12.799846 pyquil-4.9.2/pyquil/quantum_processor/qcs.py
--rw-r--r--   0        0        0      417 2024-04-17 21:33:12.799846 pyquil-4.9.2/pyquil/quantum_processor/transformers/__init__.py
--rw-r--r--   0        0        0      331 2024-04-17 21:33:12.799846 pyquil-4.9.2/pyquil/quantum_processor/transformers/compiler_isa_to_graph.py
--rw-r--r--   0        0        0     5279 2024-04-17 21:33:12.799846 pyquil-4.9.2/pyquil/quantum_processor/transformers/graph_to_compiler_isa.py
--rw-r--r--   0        0        0    11791 2024-04-17 21:33:12.799846 pyquil-4.9.2/pyquil/quantum_processor/transformers/qcs_isa_to_compiler_isa.py
--rw-r--r--   0        0        0      224 2024-04-17 21:33:12.799846 pyquil-4.9.2/pyquil/quantum_processor/transformers/qcs_isa_to_graph.py
--rw-r--r--   0        0        0    48564 2024-04-17 21:33:12.799846 pyquil-4.9.2/pyquil/quil.py
--rw-r--r--   0        0        0    44831 2024-04-17 21:33:12.799846 pyquil-4.9.2/pyquil/quilatom.py
--rw-r--r--   0        0        0   103651 2024-04-17 21:33:12.799846 pyquil-4.9.2/pyquil/quilbase.py
--rw-r--r--   0        0        0     4191 2024-04-17 21:33:12.799846 pyquil-4.9.2/pyquil/quiltcalibrations.py
--rw-r--r--   0        0        0    10338 2024-04-17 21:33:12.799846 pyquil-4.9.2/pyquil/quiltwaveforms.py
--rw-r--r--   0        0        0      511 2024-04-17 21:33:12.799846 pyquil-4.9.2/pyquil/simulation/__init__.py
--rw-r--r--   0        0        0    13329 2024-04-17 21:33:12.799846 pyquil-4.9.2/pyquil/simulation/_numpy.py
--rw-r--r--   0        0        0    15815 2024-04-17 21:33:12.799846 pyquil-4.9.2/pyquil/simulation/_reference.py
--rw-r--r--   0        0        0    14218 2024-04-17 21:33:12.799846 pyquil-4.9.2/pyquil/simulation/matrices.py
--rw-r--r--   0        0        0    19105 2024-04-17 21:33:12.799846 pyquil-4.9.2/pyquil/simulation/tools.py
--rw-r--r--   0        0        0     8766 2024-04-17 21:33:12.799846 pyquil-4.9.2/pyquil/wavefunction.py
--rw-r--r--   0        0        0    11057 1970-01-01 00:00:00.000000 pyquil-4.9.2/PKG-INFO
+-rw-r--r--   0        0        0    11358 2024-04-17 21:31:06.795572 pyquil-4.9.2rc0/LICENSE
+-rw-r--r--   0        0        0     1779 2024-04-17 21:31:06.795572 pyquil-4.9.2rc0/NOTICE.md
+-rw-r--r--   0        0        0     8944 2024-04-17 21:31:06.795572 pyquil-4.9.2rc0/README.md
+-rw-r--r--   0        0        0     2781 2024-04-17 21:31:07.035573 pyquil-4.9.2rc0/pyproject.toml
+-rw-r--r--   0        0        0      159 2024-04-17 21:31:07.035573 pyquil-4.9.2rc0/pyquil/__init__.py
+-rw-r--r--   0        0        0     1082 2024-04-17 21:31:07.035573 pyquil-4.9.2rc0/pyquil/_version.py
+-rw-r--r--   0        0        0     2129 2024-04-17 21:31:07.035573 pyquil-4.9.2rc0/pyquil/api/__init__.py
+-rw-r--r--   0        0        0     8884 2024-04-17 21:31:07.035573 pyquil-4.9.2rc0/pyquil/api/_abstract_compiler.py
+-rw-r--r--   0        0        0     7377 2024-04-17 21:31:07.035573 pyquil-4.9.2rc0/pyquil/api/_benchmark.py
+-rw-r--r--   0        0        0     9942 2024-04-17 21:31:07.035573 pyquil-4.9.2rc0/pyquil/api/_compiler.py
+-rw-r--r--   0        0        0     5554 2024-04-17 21:31:07.035573 pyquil-4.9.2rc0/pyquil/api/_compiler_client.py
+-rw-r--r--   0        0        0     4265 2024-04-17 21:31:07.035573 pyquil-4.9.2rc0/pyquil/api/_errors.py
+-rw-r--r--   0        0        0     1010 2024-04-17 21:31:07.035573 pyquil-4.9.2rc0/pyquil/api/_logger.py
+-rw-r--r--   0        0        0     7568 2024-04-17 21:31:07.035573 pyquil-4.9.2rc0/pyquil/api/_qam.py
+-rw-r--r--   0        0        0    11336 2024-04-17 21:31:07.035573 pyquil-4.9.2rc0/pyquil/api/_qpu.py
+-rw-r--r--   0        0        0    55258 2024-04-17 21:31:07.035573 pyquil-4.9.2rc0/pyquil/api/_quantum_computer.py
+-rw-r--r--   0        0        0     8637 2024-04-17 21:31:07.035573 pyquil-4.9.2rc0/pyquil/api/_qvm.py
+-rw-r--r--   0        0        0     5562 2024-04-17 21:31:07.035573 pyquil-4.9.2rc0/pyquil/api/_rewrite_arithmetic.py
+-rw-r--r--   0        0        0    10749 2024-04-17 21:31:07.035573 pyquil-4.9.2rc0/pyquil/api/_wavefunction_simulator.py
+-rw-r--r--   0        0        0      369 2024-04-17 21:31:07.035573 pyquil-4.9.2rc0/pyquil/diagnostics.py
+-rw-r--r--   0        0        0     1371 2024-04-17 21:31:07.035573 pyquil-4.9.2rc0/pyquil/experiment/__init__.py
+-rw-r--r--   0        0        0      896 2024-04-17 21:31:07.035573 pyquil-4.9.2rc0/pyquil/experiment/_calibration.py
+-rw-r--r--   0        0        0    15705 2024-04-17 21:31:07.035573 pyquil-4.9.2rc0/pyquil/experiment/_group.py
+-rw-r--r--   0        0        0    22783 2024-04-17 21:31:07.035573 pyquil-4.9.2rc0/pyquil/experiment/_main.py
+-rw-r--r--   0        0        0     8213 2024-04-17 21:31:07.039573 pyquil-4.9.2rc0/pyquil/experiment/_memory.py
+-rw-r--r--   0        0        0     5547 2024-04-17 21:31:07.039573 pyquil-4.9.2rc0/pyquil/experiment/_program.py
+-rw-r--r--   0        0        0     9047 2024-04-17 21:31:07.039573 pyquil-4.9.2rc0/pyquil/experiment/_result.py
+-rw-r--r--   0        0        0     7469 2024-04-17 21:31:07.039573 pyquil-4.9.2rc0/pyquil/experiment/_setting.py
+-rw-r--r--   0        0        0      934 2024-04-17 21:31:07.039573 pyquil-4.9.2rc0/pyquil/experiment/_symmetrization.py
+-rw-r--r--   0        0        0      282 2024-04-17 21:31:07.039573 pyquil-4.9.2rc0/pyquil/external/README.md
+-rw-r--r--   0        0        0        0 2024-04-17 21:31:07.039573 pyquil-4.9.2rc0/pyquil/external/__init__.py
+-rw-r--r--   0        0        0     9858 2024-04-17 21:31:07.039573 pyquil-4.9.2rc0/pyquil/external/rpcq.py
+-rw-r--r--   0        0        0    42387 2024-04-17 21:31:07.039573 pyquil-4.9.2rc0/pyquil/gates.py
+-rw-r--r--   0        0        0      201 2024-04-17 21:31:07.039573 pyquil-4.9.2rc0/pyquil/latex/__init__.py
+-rw-r--r--   0        0        0    18720 2024-04-17 21:31:07.039573 pyquil-4.9.2rc0/pyquil/latex/_diagram.py
+-rw-r--r--   0        0        0     3452 2024-04-17 21:31:07.039573 pyquil-4.9.2rc0/pyquil/latex/_ipython.py
+-rw-r--r--   0        0        0     4041 2024-04-17 21:31:07.039573 pyquil-4.9.2rc0/pyquil/latex/_main.py
+-rw-r--r--   0        0        0     1266 2024-04-17 21:31:07.039573 pyquil-4.9.2rc0/pyquil/latex/latex_generation.py
+-rw-r--r--   0        0        0    31958 2024-04-17 21:31:07.039573 pyquil-4.9.2rc0/pyquil/noise.py
+-rw-r--r--   0        0        0     3346 2024-04-17 21:31:07.039573 pyquil-4.9.2rc0/pyquil/noise_gates.py
+-rw-r--r--   0        0        0    15865 2024-04-17 21:31:07.039573 pyquil-4.9.2rc0/pyquil/operator_estimation.py
+-rw-r--r--   0        0        0    42310 2024-04-17 21:31:07.039573 pyquil-4.9.2rc0/pyquil/paulis.py
+-rw-r--r--   0        0        0        0 2024-04-17 21:31:07.039573 pyquil-4.9.2rc0/pyquil/py.typed
+-rw-r--r--   0        0        0    19676 2024-04-17 21:31:07.039573 pyquil-4.9.2rc0/pyquil/pyqvm.py
+-rw-r--r--   0        0        0      336 2024-04-17 21:31:07.039573 pyquil-4.9.2rc0/pyquil/quantum_processor/__init__.py
+-rw-r--r--   0        0        0     1662 2024-04-17 21:31:07.039573 pyquil-4.9.2rc0/pyquil/quantum_processor/_base.py
+-rw-r--r--   0        0        0        0 2024-04-17 21:31:07.039573 pyquil-4.9.2rc0/pyquil/quantum_processor/_isa.py
+-rw-r--r--   0        0        0      774 2024-04-17 21:31:07.039573 pyquil-4.9.2rc0/pyquil/quantum_processor/compiler.py
+-rw-r--r--   0        0        0     1856 2024-04-17 21:31:07.039573 pyquil-4.9.2rc0/pyquil/quantum_processor/graph.py
+-rw-r--r--   0        0        0     2714 2024-04-17 21:31:07.039573 pyquil-4.9.2rc0/pyquil/quantum_processor/qcs.py
+-rw-r--r--   0        0        0      417 2024-04-17 21:31:07.039573 pyquil-4.9.2rc0/pyquil/quantum_processor/transformers/__init__.py
+-rw-r--r--   0        0        0      331 2024-04-17 21:31:07.039573 pyquil-4.9.2rc0/pyquil/quantum_processor/transformers/compiler_isa_to_graph.py
+-rw-r--r--   0        0        0     5279 2024-04-17 21:31:07.039573 pyquil-4.9.2rc0/pyquil/quantum_processor/transformers/graph_to_compiler_isa.py
+-rw-r--r--   0        0        0    11791 2024-04-17 21:31:07.039573 pyquil-4.9.2rc0/pyquil/quantum_processor/transformers/qcs_isa_to_compiler_isa.py
+-rw-r--r--   0        0        0      224 2024-04-17 21:31:07.039573 pyquil-4.9.2rc0/pyquil/quantum_processor/transformers/qcs_isa_to_graph.py
+-rw-r--r--   0        0        0    48564 2024-04-17 21:31:07.039573 pyquil-4.9.2rc0/pyquil/quil.py
+-rw-r--r--   0        0        0    44831 2024-04-17 21:31:07.039573 pyquil-4.9.2rc0/pyquil/quilatom.py
+-rw-r--r--   0        0        0   103651 2024-04-17 21:31:07.039573 pyquil-4.9.2rc0/pyquil/quilbase.py
+-rw-r--r--   0        0        0     4191 2024-04-17 21:31:07.039573 pyquil-4.9.2rc0/pyquil/quiltcalibrations.py
+-rw-r--r--   0        0        0    10338 2024-04-17 21:31:07.039573 pyquil-4.9.2rc0/pyquil/quiltwaveforms.py
+-rw-r--r--   0        0        0      511 2024-04-17 21:31:07.039573 pyquil-4.9.2rc0/pyquil/simulation/__init__.py
+-rw-r--r--   0        0        0    13329 2024-04-17 21:31:07.039573 pyquil-4.9.2rc0/pyquil/simulation/_numpy.py
+-rw-r--r--   0        0        0    15815 2024-04-17 21:31:07.039573 pyquil-4.9.2rc0/pyquil/simulation/_reference.py
+-rw-r--r--   0        0        0    14218 2024-04-17 21:31:07.039573 pyquil-4.9.2rc0/pyquil/simulation/matrices.py
+-rw-r--r--   0        0        0    19105 2024-04-17 21:31:07.039573 pyquil-4.9.2rc0/pyquil/simulation/tools.py
+-rw-r--r--   0        0        0     8766 2024-04-17 21:31:07.039573 pyquil-4.9.2rc0/pyquil/wavefunction.py
+-rw-r--r--   0        0        0    11060 1970-01-01 00:00:00.000000 pyquil-4.9.2rc0/PKG-INFO
```

### Comparing `pyquil-4.9.2/LICENSE` & `pyquil-4.9.2rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyquil-4.9.2/NOTICE.md` & `pyquil-4.9.2rc0/NOTICE.md`

 * *Files identical despite different names*

### Comparing `pyquil-4.9.2/README.md` & `pyquil-4.9.2rc0/README.md`

 * *Files identical despite different names*

### Comparing `pyquil-4.9.2/pyproject.toml` & `pyquil-4.9.2rc0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyquil"
-version = "4.9.2"
+version = "4.9.2-rc.0"
 description = "A Python library for creating Quantum Instruction Language (Quil) programs."
 authors = ["Rigetti Computing <softapps@rigetti.com>"]
 readme = "README.md"
 repository = "https://github.com/rigetti/pyquil.git"
 documentation = "https://pyquil-docs.rigetti.com"
 license = "Apache-2.0"
 classifiers = [
```

### Comparing `pyquil-4.9.2/pyquil/_version.py` & `pyquil-4.9.2rc0/pyquil/_version.py`

 * *Files identical despite different names*

### Comparing `pyquil-4.9.2/pyquil/api/__init__.py` & `pyquil-4.9.2rc0/pyquil/api/__init__.py`

 * *Files identical despite different names*

### Comparing `pyquil-4.9.2/pyquil/api/_abstract_compiler.py` & `pyquil-4.9.2rc0/pyquil/api/_abstract_compiler.py`

 * *Files identical despite different names*

### Comparing `pyquil-4.9.2/pyquil/api/_benchmark.py` & `pyquil-4.9.2rc0/pyquil/api/_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyquil-4.9.2/pyquil/api/_compiler.py` & `pyquil-4.9.2rc0/pyquil/api/_compiler.py`

 * *Files identical despite different names*

### Comparing `pyquil-4.9.2/pyquil/api/_compiler_client.py` & `pyquil-4.9.2rc0/pyquil/api/_compiler_client.py`

 * *Files identical despite different names*

### Comparing `pyquil-4.9.2/pyquil/api/_errors.py` & `pyquil-4.9.2rc0/pyquil/api/_errors.py`

 * *Files identical despite different names*

### Comparing `pyquil-4.9.2/pyquil/api/_logger.py` & `pyquil-4.9.2rc0/pyquil/api/_logger.py`

 * *Files identical despite different names*

### Comparing `pyquil-4.9.2/pyquil/api/_qam.py` & `pyquil-4.9.2rc0/pyquil/api/_qam.py`

 * *Files identical despite different names*

### Comparing `pyquil-4.9.2/pyquil/api/_qpu.py` & `pyquil-4.9.2rc0/pyquil/api/_qpu.py`

 * *Files identical despite different names*

### Comparing `pyquil-4.9.2/pyquil/api/_quantum_computer.py` & `pyquil-4.9.2rc0/pyquil/api/_quantum_computer.py`

 * *Files identical despite different names*

### Comparing `pyquil-4.9.2/pyquil/api/_qvm.py` & `pyquil-4.9.2rc0/pyquil/api/_qvm.py`

 * *Files identical despite different names*

### Comparing `pyquil-4.9.2/pyquil/api/_rewrite_arithmetic.py` & `pyquil-4.9.2rc0/pyquil/api/_rewrite_arithmetic.py`

 * *Files identical despite different names*

### Comparing `pyquil-4.9.2/pyquil/api/_wavefunction_simulator.py` & `pyquil-4.9.2rc0/pyquil/api/_wavefunction_simulator.py`

 * *Files identical despite different names*

### Comparing `pyquil-4.9.2/pyquil/experiment/__init__.py` & `pyquil-4.9.2rc0/pyquil/experiment/__init__.py`

 * *Files identical despite different names*

### Comparing `pyquil-4.9.2/pyquil/experiment/_calibration.py` & `pyquil-4.9.2rc0/pyquil/experiment/_calibration.py`

 * *Files identical despite different names*

### Comparing `pyquil-4.9.2/pyquil/experiment/_group.py` & `pyquil-4.9.2rc0/pyquil/experiment/_group.py`

 * *Files identical despite different names*

### Comparing `pyquil-4.9.2/pyquil/experiment/_main.py` & `pyquil-4.9.2rc0/pyquil/experiment/_main.py`

 * *Files identical despite different names*

### Comparing `pyquil-4.9.2/pyquil/experiment/_memory.py` & `pyquil-4.9.2rc0/pyquil/experiment/_memory.py`

 * *Files identical despite different names*

### Comparing `pyquil-4.9.2/pyquil/experiment/_program.py` & `pyquil-4.9.2rc0/pyquil/experiment/_program.py`

 * *Files identical despite different names*

### Comparing `pyquil-4.9.2/pyquil/experiment/_result.py` & `pyquil-4.9.2rc0/pyquil/experiment/_result.py`

 * *Files identical despite different names*

### Comparing `pyquil-4.9.2/pyquil/experiment/_setting.py` & `pyquil-4.9.2rc0/pyquil/experiment/_setting.py`

 * *Files identical despite different names*

### Comparing `pyquil-4.9.2/pyquil/experiment/_symmetrization.py` & `pyquil-4.9.2rc0/pyquil/experiment/_symmetrization.py`

 * *Files identical despite different names*

### Comparing `pyquil-4.9.2/pyquil/external/rpcq.py` & `pyquil-4.9.2rc0/pyquil/external/rpcq.py`

 * *Files identical despite different names*

### Comparing `pyquil-4.9.2/pyquil/gates.py` & `pyquil-4.9.2rc0/pyquil/gates.py`

 * *Files identical despite different names*

### Comparing `pyquil-4.9.2/pyquil/latex/_diagram.py` & `pyquil-4.9.2rc0/pyquil/latex/_diagram.py`

 * *Files identical despite different names*

### Comparing `pyquil-4.9.2/pyquil/latex/_ipython.py` & `pyquil-4.9.2rc0/pyquil/latex/_ipython.py`

 * *Files identical despite different names*

### Comparing `pyquil-4.9.2/pyquil/latex/_main.py` & `pyquil-4.9.2rc0/pyquil/latex/_main.py`

 * *Files identical despite different names*

### Comparing `pyquil-4.9.2/pyquil/latex/latex_generation.py` & `pyquil-4.9.2rc0/pyquil/latex/latex_generation.py`

 * *Files identical despite different names*

### Comparing `pyquil-4.9.2/pyquil/noise.py` & `pyquil-4.9.2rc0/pyquil/noise.py`

 * *Files identical despite different names*

### Comparing `pyquil-4.9.2/pyquil/noise_gates.py` & `pyquil-4.9.2rc0/pyquil/noise_gates.py`

 * *Files identical despite different names*

### Comparing `pyquil-4.9.2/pyquil/operator_estimation.py` & `pyquil-4.9.2rc0/pyquil/operator_estimation.py`

 * *Files identical despite different names*

### Comparing `pyquil-4.9.2/pyquil/paulis.py` & `pyquil-4.9.2rc0/pyquil/paulis.py`

 * *Files identical despite different names*

### Comparing `pyquil-4.9.2/pyquil/pyqvm.py` & `pyquil-4.9.2rc0/pyquil/pyqvm.py`

 * *Files identical despite different names*

### Comparing `pyquil-4.9.2/pyquil/quantum_processor/_base.py` & `pyquil-4.9.2rc0/pyquil/quantum_processor/_base.py`

 * *Files identical despite different names*

### Comparing `pyquil-4.9.2/pyquil/quantum_processor/compiler.py` & `pyquil-4.9.2rc0/pyquil/quantum_processor/compiler.py`

 * *Files identical despite different names*

### Comparing `pyquil-4.9.2/pyquil/quantum_processor/graph.py` & `pyquil-4.9.2rc0/pyquil/quantum_processor/graph.py`

 * *Files identical despite different names*

### Comparing `pyquil-4.9.2/pyquil/quantum_processor/qcs.py` & `pyquil-4.9.2rc0/pyquil/quantum_processor/qcs.py`

 * *Files identical despite different names*

### Comparing `pyquil-4.9.2/pyquil/quantum_processor/transformers/graph_to_compiler_isa.py` & `pyquil-4.9.2rc0/pyquil/quantum_processor/transformers/graph_to_compiler_isa.py`

 * *Files identical despite different names*

### Comparing `pyquil-4.9.2/pyquil/quantum_processor/transformers/qcs_isa_to_compiler_isa.py` & `pyquil-4.9.2rc0/pyquil/quantum_processor/transformers/qcs_isa_to_compiler_isa.py`

 * *Files identical despite different names*

### Comparing `pyquil-4.9.2/pyquil/quil.py` & `pyquil-4.9.2rc0/pyquil/quil.py`

 * *Files identical despite different names*

### Comparing `pyquil-4.9.2/pyquil/quilatom.py` & `pyquil-4.9.2rc0/pyquil/quilatom.py`

 * *Files identical despite different names*

### Comparing `pyquil-4.9.2/pyquil/quilbase.py` & `pyquil-4.9.2rc0/pyquil/quilbase.py`

 * *Files identical despite different names*

### Comparing `pyquil-4.9.2/pyquil/quiltcalibrations.py` & `pyquil-4.9.2rc0/pyquil/quiltcalibrations.py`

 * *Files identical despite different names*

### Comparing `pyquil-4.9.2/pyquil/quiltwaveforms.py` & `pyquil-4.9.2rc0/pyquil/quiltwaveforms.py`

 * *Files identical despite different names*

### Comparing `pyquil-4.9.2/pyquil/simulation/_numpy.py` & `pyquil-4.9.2rc0/pyquil/simulation/_numpy.py`

 * *Files identical despite different names*

### Comparing `pyquil-4.9.2/pyquil/simulation/_reference.py` & `pyquil-4.9.2rc0/pyquil/simulation/_reference.py`

 * *Files identical despite different names*

### Comparing `pyquil-4.9.2/pyquil/simulation/matrices.py` & `pyquil-4.9.2rc0/pyquil/simulation/matrices.py`

 * *Files identical despite different names*

### Comparing `pyquil-4.9.2/pyquil/simulation/tools.py` & `pyquil-4.9.2rc0/pyquil/simulation/tools.py`

 * *Files identical despite different names*

### Comparing `pyquil-4.9.2/pyquil/wavefunction.py` & `pyquil-4.9.2rc0/pyquil/wavefunction.py`

 * *Files identical despite different names*

### Comparing `pyquil-4.9.2/PKG-INFO` & `pyquil-4.9.2rc0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyquil
-Version: 4.9.2
+Version: 4.9.2rc0
 Summary: A Python library for creating Quantum Instruction Language (Quil) programs.
 Home-page: https://github.com/rigetti/pyquil.git
 License: Apache-2.0
 Keywords: quantum,quil,programming,hybrid
 Author: Rigetti Computing
 Author-email: softapps@rigetti.com
 Requires-Python: >=3.8,<=3.12
```

