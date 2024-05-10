# Comparing `tmp/optimas-0.5.0.tar.gz` & `tmp/optimas-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "optimas-0.5.0.tar", last modified: Fri Mar 15 14:06:33 2024, max compression
+gzip compressed data, was "optimas-0.6.0.tar", last modified: Fri May 10 21:32:50 2024, max compression
```

## Comparing `optimas-0.5.0.tar` & `optimas-0.6.0.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:06:33.669790 optimas-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)     6094 2024-03-15 14:06:33.669790 optimas-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5010 2024-03-15 14:06:29.000000 optimas-0.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:06:33.657790 optimas-0.5.0/optimas/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-15 14:06:29.000000 optimas-0.5.0/optimas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:06:33.661790 optimas-0.5.0/optimas/core/
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-03-15 14:06:29.000000 optimas-0.5.0/optimas/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-03-15 14:06:29.000000 optimas-0.5.0/optimas/core/evaluation.py
--rw-r--r--   0 runner    (1001) docker     (127)     6316 2024-03-15 14:06:29.000000 optimas-0.5.0/optimas/core/parameter.py
--rw-r--r--   0 runner    (1001) docker     (127)      631 2024-03-15 14:06:29.000000 optimas-0.5.0/optimas/core/task.py
--rw-r--r--   0 runner    (1001) docker     (127)     7023 2024-03-15 14:06:29.000000 optimas-0.5.0/optimas/core/trial.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:06:33.661790 optimas-0.5.0/optimas/diagnostics/
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-03-15 14:06:29.000000 optimas-0.5.0/optimas/diagnostics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24820 2024-03-15 14:06:29.000000 optimas-0.5.0/optimas/diagnostics/ax_model_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    38081 2024-03-15 14:06:29.000000 optimas-0.5.0/optimas/diagnostics/exploration_diagnostics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:06:33.661790 optimas-0.5.0/optimas/evaluators/
--rw-r--r--   0 runner    (1001) docker     (127)      310 2024-03-15 14:06:29.000000 optimas-0.5.0/optimas/evaluators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3718 2024-03-15 14:06:29.000000 optimas-0.5.0/optimas/evaluators/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4034 2024-03-15 14:06:29.000000 optimas-0.5.0/optimas/evaluators/chain_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-03-15 14:06:29.000000 optimas-0.5.0/optimas/evaluators/function_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3998 2024-03-15 14:06:29.000000 optimas-0.5.0/optimas/evaluators/multitask_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (127)     6318 2024-03-15 14:06:29.000000 optimas-0.5.0/optimas/evaluators/template_evaluator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:06:33.661790 optimas-0.5.0/optimas/explorations/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-03-15 14:06:29.000000 optimas-0.5.0/optimas/explorations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25165 2024-03-15 14:06:29.000000 optimas-0.5.0/optimas/explorations/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5346 2024-03-15 14:06:29.000000 optimas-0.5.0/optimas/gen_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:06:33.661790 optimas-0.5.0/optimas/generators/
--rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-03-15 14:06:29.000000 optimas-0.5.0/optimas/generators/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:06:33.661790 optimas-0.5.0/optimas/generators/ax/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 14:06:29.000000 optimas-0.5.0/optimas/generators/ax/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4193 2024-03-15 14:06:29.000000 optimas-0.5.0/optimas/generators/ax/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:06:33.665790 optimas-0.5.0/optimas/generators/ax/developer/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 14:06:29.000000 optimas-0.5.0/optimas/generators/ax/developer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      900 2024-03-15 14:06:29.000000 optimas-0.5.0/optimas/generators/ax/developer/ax_metric.py
--rw-r--r--   0 runner    (1001) docker     (127)    19394 2024-03-15 14:06:29.000000 optimas-0.5.0/optimas/generators/ax/developer/multitask.py
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-03-15 14:06:29.000000 optimas-0.5.0/optimas/generators/ax/import_error_dummy_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:06:33.665790 optimas-0.5.0/optimas/generators/ax/service/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 14:06:29.000000 optimas-0.5.0/optimas/generators/ax/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6369 2024-03-15 14:06:29.000000 optimas-0.5.0/optimas/generators/ax/service/ax_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    13266 2024-03-15 14:06:29.000000 optimas-0.5.0/optimas/generators/ax/service/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5791 2024-03-15 14:06:29.000000 optimas-0.5.0/optimas/generators/ax/service/custom_ax.py
--rw-r--r--   0 runner    (1001) docker     (127)     5430 2024-03-15 14:06:29.000000 optimas-0.5.0/optimas/generators/ax/service/multi_fidelity.py
--rw-r--r--   0 runner    (1001) docker     (127)     7516 2024-03-15 14:06:29.000000 optimas-0.5.0/optimas/generators/ax/service/single_fidelity.py
--rw-r--r--   0 runner    (1001) docker     (127)    24398 2024-03-15 14:06:29.000000 optimas-0.5.0/optimas/generators/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3163 2024-03-15 14:06:29.000000 optimas-0.5.0/optimas/generators/grid_sampling.py
--rw-r--r--   0 runner    (1001) docker     (127)     4588 2024-03-15 14:06:29.000000 optimas-0.5.0/optimas/generators/line_sampling.py
--rw-r--r--   0 runner    (1001) docker     (127)     4162 2024-03-15 14:06:29.000000 optimas-0.5.0/optimas/generators/random_sampling.py
--rw-r--r--   0 runner    (1001) docker     (127)     5740 2024-03-15 14:06:29.000000 optimas-0.5.0/optimas/sim_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:06:33.665790 optimas-0.5.0/optimas/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 14:06:29.000000 optimas-0.5.0/optimas/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      795 2024-03-15 14:06:29.000000 optimas-0.5.0/optimas/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     3324 2024-03-15 14:06:29.000000 optimas-0.5.0/optimas/utils/other.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:06:33.669790 optimas-0.5.0/optimas.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6094 2024-03-15 14:06:33.000000 optimas-0.5.0/optimas.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-03-15 14:06:33.000000 optimas-0.5.0/optimas.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-15 14:06:33.000000 optimas-0.5.0/optimas.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-03-15 14:06:33.000000 optimas-0.5.0/optimas.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-15 14:06:33.000000 optimas-0.5.0/optimas.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-03-15 14:06:29.000000 optimas-0.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-15 14:06:33.669790 optimas-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-15 14:06:29.000000 optimas-0.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:06:33.669790 optimas-0.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3937 2024-03-15 14:06:29.000000 optimas-0.5.0/tests/test_analyzed_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)    23525 2024-03-15 14:06:29.000000 optimas-0.5.0/tests/test_ax_generators.py
--rw-r--r--   0 runner    (1001) docker     (127)     5178 2024-03-15 14:06:29.000000 optimas-0.5.0/tests/test_ax_model_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     3615 2024-03-15 14:06:29.000000 optimas-0.5.0/tests/test_chain_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-03-15 14:06:29.000000 optimas-0.5.0/tests/test_comms.py
--rw-r--r--   0 runner    (1001) docker     (127)     1820 2024-03-15 14:06:29.000000 optimas-0.5.0/tests/test_env_script.py
--rw-r--r--   0 runner    (1001) docker     (127)     6130 2024-03-15 14:06:29.000000 optimas-0.5.0/tests/test_exploration_diagnostics.py
--rw-r--r--   0 runner    (1001) docker     (127)     4984 2024-03-15 14:06:29.000000 optimas-0.5.0/tests/test_exploration_resume.py
--rw-r--r--   0 runner    (1001) docker     (127)     2382 2024-03-15 14:06:29.000000 optimas-0.5.0/tests/test_function_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-03-15 14:06:29.000000 optimas-0.5.0/tests/test_grid_sampling.py
--rw-r--r--   0 runner    (1001) docker     (127)     3446 2024-03-15 14:06:29.000000 optimas-0.5.0/tests/test_line_sampling.py
--rw-r--r--   0 runner    (1001) docker     (127)     4660 2024-03-15 14:06:29.000000 optimas-0.5.0/tests/test_manual_exploration.py
--rw-r--r--   0 runner    (1001) docker     (127)     3532 2024-03-15 14:06:29.000000 optimas-0.5.0/tests/test_random_sampling.py
--rw-r--r--   0 runner    (1001) docker     (127)     3950 2024-03-15 14:06:29.000000 optimas-0.5.0/tests/test_template_evaluator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 21:32:50.299115 optimas-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     6046 2024-05-10 21:32:50.299115 optimas-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5009 2024-05-10 21:32:46.000000 optimas-0.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 21:32:50.287115 optimas-0.6.0/optimas/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-10 21:32:46.000000 optimas-0.6.0/optimas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 21:32:50.291115 optimas-0.6.0/optimas/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-05-10 21:32:46.000000 optimas-0.6.0/optimas/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-10 21:32:46.000000 optimas-0.6.0/optimas/core/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6316 2024-05-10 21:32:46.000000 optimas-0.6.0/optimas/core/parameter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2024-05-10 21:32:46.000000 optimas-0.6.0/optimas/core/task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7023 2024-05-10 21:32:46.000000 optimas-0.6.0/optimas/core/trial.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 21:32:50.291115 optimas-0.6.0/optimas/diagnostics/
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-10 21:32:46.000000 optimas-0.6.0/optimas/diagnostics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24818 2024-05-10 21:32:46.000000 optimas-0.6.0/optimas/diagnostics/ax_model_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38001 2024-05-10 21:32:46.000000 optimas-0.6.0/optimas/diagnostics/exploration_diagnostics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 21:32:50.291115 optimas-0.6.0/optimas/evaluators/
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-05-10 21:32:46.000000 optimas-0.6.0/optimas/evaluators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3718 2024-05-10 21:32:46.000000 optimas-0.6.0/optimas/evaluators/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4034 2024-05-10 21:32:46.000000 optimas-0.6.0/optimas/evaluators/chain_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-05-10 21:32:46.000000 optimas-0.6.0/optimas/evaluators/function_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3998 2024-05-10 21:32:46.000000 optimas-0.6.0/optimas/evaluators/multitask_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6318 2024-05-10 21:32:46.000000 optimas-0.6.0/optimas/evaluators/template_evaluator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 21:32:50.291115 optimas-0.6.0/optimas/explorations/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-10 21:32:46.000000 optimas-0.6.0/optimas/explorations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25219 2024-05-10 21:32:46.000000 optimas-0.6.0/optimas/explorations/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5225 2024-05-10 21:32:46.000000 optimas-0.6.0/optimas/gen_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 21:32:50.291115 optimas-0.6.0/optimas/generators/
+-rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-05-10 21:32:46.000000 optimas-0.6.0/optimas/generators/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 21:32:50.291115 optimas-0.6.0/optimas/generators/ax/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 21:32:46.000000 optimas-0.6.0/optimas/generators/ax/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4193 2024-05-10 21:32:46.000000 optimas-0.6.0/optimas/generators/ax/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 21:32:50.295115 optimas-0.6.0/optimas/generators/ax/developer/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 21:32:46.000000 optimas-0.6.0/optimas/generators/ax/developer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      900 2024-05-10 21:32:46.000000 optimas-0.6.0/optimas/generators/ax/developer/ax_metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18644 2024-05-10 21:32:46.000000 optimas-0.6.0/optimas/generators/ax/developer/multitask.py
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-10 21:32:46.000000 optimas-0.6.0/optimas/generators/ax/import_error_dummy_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 21:32:50.295115 optimas-0.6.0/optimas/generators/ax/service/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 21:32:46.000000 optimas-0.6.0/optimas/generators/ax/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6369 2024-05-10 21:32:46.000000 optimas-0.6.0/optimas/generators/ax/service/ax_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11696 2024-05-10 21:32:46.000000 optimas-0.6.0/optimas/generators/ax/service/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5857 2024-05-10 21:32:46.000000 optimas-0.6.0/optimas/generators/ax/service/multi_fidelity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7516 2024-05-10 21:32:46.000000 optimas-0.6.0/optimas/generators/ax/service/single_fidelity.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23009 2024-05-10 21:32:46.000000 optimas-0.6.0/optimas/generators/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3163 2024-05-10 21:32:46.000000 optimas-0.6.0/optimas/generators/grid_sampling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4588 2024-05-10 21:32:46.000000 optimas-0.6.0/optimas/generators/line_sampling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4162 2024-05-10 21:32:46.000000 optimas-0.6.0/optimas/generators/random_sampling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5740 2024-05-10 21:32:46.000000 optimas-0.6.0/optimas/sim_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 21:32:50.295115 optimas-0.6.0/optimas/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 21:32:46.000000 optimas-0.6.0/optimas/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-05-10 21:32:46.000000 optimas-0.6.0/optimas/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2728 2024-05-10 21:32:46.000000 optimas-0.6.0/optimas/utils/other.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 21:32:50.299115 optimas-0.6.0/optimas.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6046 2024-05-10 21:32:50.000000 optimas-0.6.0/optimas.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-05-10 21:32:50.000000 optimas-0.6.0/optimas.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 21:32:50.000000 optimas-0.6.0/optimas.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-10 21:32:50.000000 optimas-0.6.0/optimas.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-10 21:32:50.000000 optimas-0.6.0/optimas.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-05-10 21:32:46.000000 optimas-0.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 21:32:50.299115 optimas-0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 21:32:46.000000 optimas-0.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 21:32:50.295115 optimas-0.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3937 2024-05-10 21:32:46.000000 optimas-0.6.0/tests/test_analyzed_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23921 2024-05-10 21:32:46.000000 optimas-0.6.0/tests/test_ax_generators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5178 2024-05-10 21:32:46.000000 optimas-0.6.0/tests/test_ax_model_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3615 2024-05-10 21:32:46.000000 optimas-0.6.0/tests/test_chain_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-05-10 21:32:46.000000 optimas-0.6.0/tests/test_comms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1820 2024-05-10 21:32:46.000000 optimas-0.6.0/tests/test_env_script.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6130 2024-05-10 21:32:46.000000 optimas-0.6.0/tests/test_exploration_diagnostics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4984 2024-05-10 21:32:46.000000 optimas-0.6.0/tests/test_exploration_resume.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3378 2024-05-10 21:32:46.000000 optimas-0.6.0/tests/test_function_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4963 2024-05-10 21:32:46.000000 optimas-0.6.0/tests/test_gpu_resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-05-10 21:32:46.000000 optimas-0.6.0/tests/test_grid_sampling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3446 2024-05-10 21:32:46.000000 optimas-0.6.0/tests/test_line_sampling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4660 2024-05-10 21:32:46.000000 optimas-0.6.0/tests/test_manual_exploration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3532 2024-05-10 21:32:46.000000 optimas-0.6.0/tests/test_random_sampling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3950 2024-05-10 21:32:46.000000 optimas-0.6.0/tests/test_template_evaluator.py
```

### Comparing `optimas-0.5.0/PKG-INFO` & `optimas-0.6.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,36 +1,35 @@
 Metadata-Version: 2.1
 Name: optimas
-Version: 0.5.0
+Version: 0.6.0
 Summary: Optimization at scale, powered by libEnsemble
 Author-email: Optimas Developers <angel.ferran.pousa@desy.de>
 License: BSD-3-Clause-LBNL
 Project-URL: Documentation, https://optimas.readthedocs.io/
 Keywords: optimization,scale,bayesian
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.9
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
-Requires-Dist: libensemble>=1.2
+Requires-Dist: libensemble>=1.3.0
 Requires-Dist: jinja2
 Requires-Dist: pandas
 Requires-Dist: mpi4py
 Requires-Dist: pydantic>=2.0
 Provides-Extra: test
 Requires-Dist: flake8; extra == "test"
 Requires-Dist: pytest; extra == "test"
-Requires-Dist: ax-platform>=0.3.4; extra == "test"
+Requires-Dist: ax-platform>=0.4.0; extra == "test"
 Requires-Dist: matplotlib; extra == "test"
 Provides-Extra: all
-Requires-Dist: ax-platform>=0.3.4; extra == "all"
+Requires-Dist: ax-platform>=0.4.0; extra == "all"
 
 [![PyPI](https://img.shields.io/pypi/v/optimas)](https://pypi.org/project/optimas/)
 [![Conda Version](https://img.shields.io/conda/vn/conda-forge/optimas.svg)](https://anaconda.org/conda-forge/optimas)
 [![tests badge](https://github.com/optimas-org/optimas/actions/workflows/unix.yml/badge.svg)](https://github.com/optimas-org/optimas/actions)
 [![Documentation Status](https://readthedocs.org/projects/optimas/badge/?version=latest)](https://optimas.readthedocs.io/en/latest/?badge=latest)
 [![DOI](https://zenodo.org/badge/287560975.svg)](https://zenodo.org/badge/latestdoi/287560975)
 [![License](https://img.shields.io/pypi/l/optimas.svg)](license.txt)
@@ -78,15 +77,15 @@
 ```sh
 conda install optimas --channel conda-forge
 ```
 or directly from GitHub:
 ```sh
 pip install git+https://github.com/optimas-org/optimas.git
 ```
-Make sure `mpi4py` is available in your environment before installing optimas. Fore more details, check out the full [installation guide](https://optimas.readthedocs.io/en/latest/user_guide/installation_local.html). We have also prepared dedicated installation instructions for some HPC systems such as
+Make sure `mpi4py` is available in your environment before installing optimas. For more details, check out the full [installation guide](https://optimas.readthedocs.io/en/latest/user_guide/installation_local.html). We have also prepared dedicated installation instructions for some HPC systems such as
 [JUWELS (JSC)](https://optimas.readthedocs.io/en/latest/user_guide/installation_juwels.html),
 [Maxwell (DESY)](https://optimas.readthedocs.io/en/latest/user_guide/installation_maxwell.html) and
 [Perlmutter (NERSC)](https://optimas.readthedocs.io/en/latest/user_guide/installation_perlmutter.html).
 
 
 ## Documentation
 For more information on how to use Optimas, check out the [documentation](https://optimas.readthedocs.io/). You'll find installation instructions, a user guide, [examples](https://optimas.readthedocs.io/en/latest/examples/index.html) and the API reference.
```

#### html2text {}

```diff
@@ -1,31 +1,30 @@
-Metadata-Version: 2.1 Name: optimas Version: 0.5.0 Summary: Optimization at
+Metadata-Version: 2.1 Name: optimas Version: 0.6.0 Summary: Optimization at
 scale, powered by libEnsemble Author-email: Optimas Developers
 desy.de> License: BSD-3-Clause-LBNL Project-URL: Documentation, https://
 optimas.readthedocs.io/ Keywords: optimization,scale,bayesian Classifier:
 Development Status :: 3 - Alpha Classifier: Intended Audience :: Science/
 Research Classifier: Topic :: Scientific/Engineering Classifier: Operating
-System :: OS Independent Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
-Language :: Python :: 3.11 Requires-Python: >=3.9 Description-Content-Type:
-text/markdown Requires-Dist: libensemble>=1.2 Requires-Dist: jinja2 Requires-
-Dist: pandas Requires-Dist: mpi4py Requires-Dist: pydantic>=2.0 Provides-Extra:
-test Requires-Dist: flake8; extra == "test" Requires-Dist: pytest; extra ==
-"test" Requires-Dist: ax-platform>=0.3.4; extra == "test" Requires-Dist:
-matplotlib; extra == "test" Provides-Extra: all Requires-Dist: ax-
-platform>=0.3.4; extra == "all" [![PyPI](https://img.shields.io/pypi/v/
-optimas)](https://pypi.org/project/optimas/) [![Conda Version](https://
-img.shields.io/conda/vn/conda-forge/optimas.svg)](https://anaconda.org/conda-
-forge/optimas) [![tests badge](https://github.com/optimas-org/optimas/actions/
-workflows/unix.yml/badge.svg)](https://github.com/optimas-org/optimas/actions)
-[![Documentation Status](https://readthedocs.org/projects/optimas/badge/
-?version=latest)](https://optimas.readthedocs.io/en/latest/?badge=latest) [!
-[DOI](https://zenodo.org/badge/287560975.svg)](https://zenodo.org/badge/
-latestdoi/287560975) [![License](https://img.shields.io/pypi/l/optimas.svg)]
-(license.txt)
+System :: OS Independent Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11 Requires-Python: >=3.10
+Description-Content-Type: text/markdown Requires-Dist: libensemble>=1.3.0
+Requires-Dist: jinja2 Requires-Dist: pandas Requires-Dist: mpi4py Requires-
+Dist: pydantic>=2.0 Provides-Extra: test Requires-Dist: flake8; extra == "test"
+Requires-Dist: pytest; extra == "test" Requires-Dist: ax-platform>=0.4.0; extra
+== "test" Requires-Dist: matplotlib; extra == "test" Provides-Extra: all
+Requires-Dist: ax-platform>=0.4.0; extra == "all" [![PyPI](https://
+img.shields.io/pypi/v/optimas)](https://pypi.org/project/optimas/) [![Conda
+Version](https://img.shields.io/conda/vn/conda-forge/optimas.svg)](https://
+anaconda.org/conda-forge/optimas) [![tests badge](https://github.com/optimas-
+org/optimas/actions/workflows/unix.yml/badge.svg)](https://github.com/optimas-
+org/optimas/actions) [![Documentation Status](https://readthedocs.org/projects/
+optimas/badge/?version=latest)](https://optimas.readthedocs.io/en/latest/
+?badge=latest) [![DOI](https://zenodo.org/badge/287560975.svg)](https://
+zenodo.org/badge/latestdoi/287560975) [![License](https://img.shields.io/pypi/
+l/optimas.svg)](license.txt)
                                 _[_o_p_t_i_m_a_s_ _l_o_g_o_]
             ******** OOppttiimmiizzaattiioonn aatt ssccaallee,, ppoowweerreedd bbyy _ll_ii_bb_EE_nn_ss_ee_mm_bb_ll_ee ********
                              _EE_xx_pp_ll_oo_rr_ee_ _tt_hh_ee_ _dd_oo_cc_ss_ _?Â_?»
 
                    _V_i_e_w_ _E_x_a_m_p_l_e_s Â· _S_u_p_p_o_r_t Â· _A_P_I_ _R_e_f_e_r_e_n_c_e
 Optimas is a Python library designed for highly scalable optimization, from
 laptops to massively-parallel supercomputers. ## Key Features -
@@ -38,15 +37,15 @@
 **Advanced Optimization**: Optimas integrates algorithms from the [Ax](https://
 github.com/facebook/Ax) library, offering both single- and multi-objective
 Bayesian optimization. This includes advanced techniques such as multi-fidelity
 and multi-task algorithms. ## Installation You can install Optimas from PyPI
 (recommended): ```sh pip install optimas ``` from conda-forge: ```sh conda
 install optimas --channel conda-forge ``` or directly from GitHub: ```sh pip
 install git+https://github.com/optimas-org/optimas.git ``` Make sure `mpi4py`
-is available in your environment before installing optimas. Fore more details,
+is available in your environment before installing optimas. For more details,
 check out the full [installation guide](https://optimas.readthedocs.io/en/
 latest/user_guide/installation_local.html). We have also prepared dedicated
 installation instructions for some HPC systems such as [JUWELS (JSC)](https://
 optimas.readthedocs.io/en/latest/user_guide/installation_juwels.html), [Maxwell
 (DESY)](https://optimas.readthedocs.io/en/latest/user_guide/
 installation_maxwell.html) and [Perlmutter (NERSC)](https://
 optimas.readthedocs.io/en/latest/user_guide/installation_perlmutter.html). ##
```

### Comparing `optimas-0.5.0/README.md` & `optimas-0.6.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 ```sh
 conda install optimas --channel conda-forge
 ```
 or directly from GitHub:
 ```sh
 pip install git+https://github.com/optimas-org/optimas.git
 ```
-Make sure `mpi4py` is available in your environment before installing optimas. Fore more details, check out the full [installation guide](https://optimas.readthedocs.io/en/latest/user_guide/installation_local.html). We have also prepared dedicated installation instructions for some HPC systems such as
+Make sure `mpi4py` is available in your environment before installing optimas. For more details, check out the full [installation guide](https://optimas.readthedocs.io/en/latest/user_guide/installation_local.html). We have also prepared dedicated installation instructions for some HPC systems such as
 [JUWELS (JSC)](https://optimas.readthedocs.io/en/latest/user_guide/installation_juwels.html),
 [Maxwell (DESY)](https://optimas.readthedocs.io/en/latest/user_guide/installation_maxwell.html) and
 [Perlmutter (NERSC)](https://optimas.readthedocs.io/en/latest/user_guide/installation_perlmutter.html).
 
 
 ## Documentation
 For more information on how to use Optimas, check out the [documentation](https://optimas.readthedocs.io/). You'll find installation instructions, a user guide, [examples](https://optimas.readthedocs.io/en/latest/examples/index.html) and the API reference.
```

#### html2text {}

```diff
@@ -23,15 +23,15 @@
 **Advanced Optimization**: Optimas integrates algorithms from the [Ax](https://
 github.com/facebook/Ax) library, offering both single- and multi-objective
 Bayesian optimization. This includes advanced techniques such as multi-fidelity
 and multi-task algorithms. ## Installation You can install Optimas from PyPI
 (recommended): ```sh pip install optimas ``` from conda-forge: ```sh conda
 install optimas --channel conda-forge ``` or directly from GitHub: ```sh pip
 install git+https://github.com/optimas-org/optimas.git ``` Make sure `mpi4py`
-is available in your environment before installing optimas. Fore more details,
+is available in your environment before installing optimas. For more details,
 check out the full [installation guide](https://optimas.readthedocs.io/en/
 latest/user_guide/installation_local.html). We have also prepared dedicated
 installation instructions for some HPC systems such as [JUWELS (JSC)](https://
 optimas.readthedocs.io/en/latest/user_guide/installation_juwels.html), [Maxwell
 (DESY)](https://optimas.readthedocs.io/en/latest/user_guide/
 installation_maxwell.html) and [Perlmutter (NERSC)](https://
 optimas.readthedocs.io/en/latest/user_guide/installation_perlmutter.html). ##
```

### Comparing `optimas-0.5.0/optimas/core/evaluation.py` & `optimas-0.6.0/optimas/core/evaluation.py`

 * *Files identical despite different names*

### Comparing `optimas-0.5.0/optimas/core/parameter.py` & `optimas-0.6.0/optimas/core/parameter.py`

 * *Files identical despite different names*

### Comparing `optimas-0.5.0/optimas/core/task.py` & `optimas-0.6.0/optimas/core/task.py`

 * *Files identical despite different names*

### Comparing `optimas-0.5.0/optimas/core/trial.py` & `optimas-0.6.0/optimas/core/trial.py`

 * *Files identical despite different names*

### Comparing `optimas-0.5.0/optimas/diagnostics/ax_model_manager.py` & `optimas-0.6.0/optimas/diagnostics/ax_model_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -435,15 +435,15 @@
         if range_x[1] is None:
             range_x[1] = experiment.parameters[param_x].upper
         if range_y[0] is None:
             range_y[0] = experiment.parameters[param_y].lower
         if range_y[1] is None:
             range_y[1] = experiment.parameters[param_y].upper
 
-        # get grid sample of points where to evalutate the model
+        # get grid sample of points where to evaluate the model
         xaxis = np.linspace(range_x[0], range_x[1], n_points)
         yaxis = np.linspace(range_y[0], range_y[1], n_points)
         X, Y = np.meshgrid(xaxis, yaxis)
         sample = {param_x: X.flatten(), param_y: Y.flatten()}
 
         if slice_values == "mid":
             # Get mid point
@@ -592,15 +592,15 @@
         if range is None:
             range = [None, None]
         if range[0] is None:
             range[0] = experiment.parameters[param_name].lower
         if range[1] is None:
             range[1] = experiment.parameters[param_name].upper
 
-        # get sample of points where to evalutate the model
+        # get sample of points where to evaluate the model
         sample = {param_name: np.linspace(range[0], range[1], n_points)}
 
         if slice_values == "mid":
             # Get mid point
             slice_values = self._get_mid_point()
         elif slice_values == "best":
             # get best point
```

### Comparing `optimas-0.5.0/optimas/diagnostics/exploration_diagnostics.py` & `optimas-0.6.0/optimas/diagnostics/exploration_diagnostics.py`

 * *Files 1% similar despite different names*

```diff
@@ -485,15 +485,16 @@
         """
         try:
             return self._sim_dir_paths[trial_index]
         except KeyError:
             raise ValueError(
                 f"Could not find evaluation directory of trial {trial_index}."
                 "This directory is only created when using a "
-                "`TemplateEvaluator`."
+                "`TemplateEvaluator` or a `FunctionEvaluator` when setting "
+                "`create_evaluation_dirs=True`."
             )
 
     def get_best_evaluation_dir_path(
         self, objective: Optional[Union[str, Objective]] = None
     ) -> str:
         """Get the path to the directory of the best evaluation.
 
@@ -611,15 +612,15 @@
             'f' : [None, -10.] (get data with f < -10)
         sort: dict, optional
             A dict containing as keys the names of the parameres to sort by
             and, as values, a Bool indicating if ordering ascendingly (True)
             or descendingly (False)
             e.g. {'f': False} sort simulations according to f descendingly.
         top: int, optional
-            Highight the 'top' evaluations of every objective.
+            Highlight the 'top' evaluations of every objective.
         show_top_evaluation_indices : bool, optional
             Whether to show the indices of the top evaluations.
         show_legend : bool, optional
             Whether to show the legend.
         subplot_spec: SubplotSpec, optional
             The location of the plot in the GridSpec of an existing figure.
             If not given, a new figure will be created.
@@ -787,28 +788,23 @@
                         orientation="horizontal",
                         label=label,
                     )
 
             ax_histy.set_ylim(ax_scatter.get_ylim())
 
             # Tuning axes and labels
-            ax_scatter.set_title(
-                parnames[i].replace("_", " "),
-                fontdict={"fontsize": "x-small"},
-                loc="right",
-                pad=2,
-            )
+            ax_scatter.set_ylabel(parnames[i])
 
             if i != nplots - 1:
                 ax_scatter.tick_params(labelbottom=False)
                 ax_histy.tick_params(labelbottom=False, labelleft=False)
             else:
                 ax_scatter.set_xlabel("Evaluation number")
                 if xname is not None:
-                    ax_scatter.set_xlabel(xname.replace("_", " "))
+                    ax_scatter.set_xlabel(xname)
                 ax_histy.set_xlabel("%")
                 ax_histy.tick_params(labelbottom=True, labelleft=False)
                 if show_legend:
                     ax_histy.legend(fontsize="xx-small")
 
             # Make loist of histograms and axes for further manipulation
             # outside the loop
```

### Comparing `optimas-0.5.0/optimas/evaluators/base.py` & `optimas-0.6.0/optimas/evaluators/base.py`

 * *Files identical despite different names*

### Comparing `optimas-0.5.0/optimas/evaluators/chain_evaluator.py` & `optimas-0.6.0/optimas/evaluators/chain_evaluator.py`

 * *Files identical despite different names*

### Comparing `optimas-0.5.0/optimas/evaluators/multitask_evaluator.py` & `optimas-0.6.0/optimas/evaluators/multitask_evaluator.py`

 * *Files identical despite different names*

### Comparing `optimas-0.5.0/optimas/evaluators/template_evaluator.py` & `optimas-0.6.0/optimas/evaluators/template_evaluator.py`

 * *Files identical despite different names*

### Comparing `optimas-0.5.0/optimas/explorations/base.py` & `optimas-0.6.0/optimas/explorations/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -169,22 +169,22 @@
         if np.isfinite(sim_max):
             exit_criteria["sim_max"] = sim_max
 
         # Get initial number of generator trials.
         n_evals_initial = self.generator.n_evaluated_trials
 
         # Create persis_info.
-        persis_info = add_unique_random_streams({}, self.sim_workers + 2)
+        persis_info = add_unique_random_streams({}, self.sim_workers + 1)
 
         # If specified, allocate dedicated resources for the generator.
         if self.generator.dedicated_resources and self.generator.use_cuda:
             persis_info["gen_resources"] = 1
             persis_info["gen_use_gpus"] = True
-        else:
-            self.libE_specs["zero_resource_workers"] = [1]
+            # Create additional resource set for generator.
+            self.libE_specs["num_resource_sets"] = self.sim_workers + 1
 
         if self._n_evals > 0:
             self.libE_specs["reuse_output_dir"] = True
 
         # Get gen_specs and sim_specs.
         run_params = self.evaluator.get_run_params()
         gen_specs = self.generator.get_gen_specs(
@@ -209,17 +209,14 @@
             self.libE_specs,
             H0=self._libe_history.H,
         )
 
         # Update history.
         self._libe_history.H = history
 
-        # Update generator with the one received from libE.
-        self.generator._update(persis_info[1]["generator"])
-
         # Update number of evaluation in this exploration.
         n_evals_final = self.generator.n_evaluated_trials
         self._n_evals += n_evals_final - n_evals_initial
 
         # Reset `cwd` to initial value before `libE` was called.
         os.chdir(cwd)
 
@@ -531,23 +528,25 @@
         )
         if history_files:
             return history_files[-1]
 
     def _set_default_libe_specs(self) -> None:
         """Set default exploration libe_specs."""
         libE_specs = {}
+        # Run generator on manager to avoid copying gen to another process.
+        libE_specs["gen_on_manager"] = True
         # Save H to file every N simulation evaluations
         # default value, if not defined
         libE_specs["save_every_k_sims"] = self.history_save_period
         # Force central mode
         libE_specs["dedicated_mode"] = False
         # Set communications and corresponding number of workers.
         libE_specs["comms"] = self.libe_comms
         if self.libe_comms in ["local", "threads"]:
-            libE_specs["nworkers"] = self.sim_workers + 1
+            libE_specs["nworkers"] = self.sim_workers
         elif self.libe_comms == "mpi":
             # Warn user if openmpi is being used.
             # When running with MPI communications, openmpi cannot be used as
             # it does not support nesting MPI.
             # MPI is only imported here to avoid issues with openmpi when
             # running with local communications.
             from mpi4py import MPI
```

### Comparing `optimas-0.5.0/optimas/gen_functions.py` & `optimas-0.6.0/optimas/gen_functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -113,12 +113,8 @@
                 generator.tell([trial])
             # Set the number of points to generate to that number:
             number_of_gen_points = min(n + n_failed_gens, max_evals - n_gens)
             n_failed_gens = 0
         else:
             number_of_gen_points = 0
 
-    # Add updated generator to `persis_info`.
-    generator._prepare_to_send()
-    persis_info["generator"] = generator
-
     return H_o, persis_info, FINISHED_PERSISTENT_GEN_TAG
```

### Comparing `optimas-0.5.0/optimas/generators/__init__.py` & `optimas-0.6.0/optimas/generators/__init__.py`

 * *Files identical despite different names*

### Comparing `optimas-0.5.0/optimas/generators/ax/base.py` & `optimas-0.6.0/optimas/generators/ax/base.py`

 * *Files identical despite different names*

### Comparing `optimas-0.5.0/optimas/generators/ax/developer/ax_metric.py` & `optimas-0.6.0/optimas/generators/ax/developer/ax_metric.py`

 * *Files identical despite different names*

### Comparing `optimas-0.5.0/optimas/generators/ax/developer/multitask.py` & `optimas-0.6.0/optimas/generators/ax/developer/multitask.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,20 +19,15 @@
 from ax.runners import SyntheticRunner
 from ax.modelbridge.factory import get_sobol
 from ax.modelbridge.torch import TorchModelBridge
 from ax.core.observation import ObservationFeatures
 from ax.core.generator_run import GeneratorRun
 from ax.storage.json_store.save import save_experiment
 from ax.storage.metric_registry import register_metric
-
-try:
-    from ax.modelbridge.factory import get_MTGP
-except ImportError:
-    # For Ax >= 0.3.4
-    from ax.modelbridge.factory import get_MTGP_LEGACY as get_MTGP
+from ax.modelbridge.factory import get_MTGP_LEGACY as get_MTGP
 
 from optimas.generators.ax.base import AxGenerator
 from optimas.core import (
     TrialParameter,
     VaryingParameter,
     Objective,
     Parameter,
@@ -351,28 +346,19 @@
                 dtype=torch.double,
                 device=torch.device(self.torch_device),
             )
             n_gen = self.lofi_task.n_opt
 
             generator_success = True
             while True:
-                if version.parse(ax_version) >= version.parse("0.3.5"):
-                    model_gen_options = {
-                        "optimizer_kwargs": {
-                            "options": {
-                                "init_batch_limit": self.init_batch_limit
-                            }
-                        }
-                    }
-                else:
-                    model_gen_options = {
-                        "optimizer_kwargs": {
-                            "init_batch_limit": self.init_batch_limit
-                        }
+                model_gen_options = {
+                    "optimizer_kwargs": {
+                        "options": {"init_batch_limit": self.init_batch_limit}
                     }
+                }
                 try:
                     # Try to generate the new points.
                     gr = m.gen(
                         n=n_gen,
                         optimization_config=(
                             self._experiment.optimization_config
                         ),
@@ -459,23 +445,14 @@
         )
         save_experiment(
             experiment=self._experiment,
             filepath=file_path,
             encoder_registry=self._encoder_registry,
         )
 
-    def _prepare_to_send(self) -> None:
-        """Prepare generator to send to another process.
-
-        Delete stored generator run. It can contain pytorch tensors that
-        prevent serialization.
-        """
-        del self.gr_lofi
-        self.gr_lofi = None
-
 
 def max_utility_from_GP(
     n: int, m: TorchModelBridge, gr: GeneratorRun, hifi_task: str
 ) -> GeneratorRun:
     """Select the max utility points according to the MTGP predictions.
 
     High fidelity batches are constructed by selecting the maximum utility
```

### Comparing `optimas-0.5.0/optimas/generators/ax/import_error_dummy_generator.py` & `optimas-0.6.0/optimas/generators/ax/import_error_dummy_generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,9 +8,9 @@
     when Ax is not installed
     """
 
     def __init__(self, *args, **kwargs) -> None:
         raise RuntimeError(
             "You need to install ax-platform, in order "
             "to use Ax-based generators in optimas.\n"
-            "e.g. with `pip install ax-platform >= 0.3.4`"
+            "e.g. with `pip install ax-platform >= 0.4.0`"
         )
```

### Comparing `optimas-0.5.0/optimas/generators/ax/service/ax_client.py` & `optimas-0.6.0/optimas/generators/ax/service/ax_client.py`

 * *Files identical despite different names*

### Comparing `optimas-0.5.0/optimas/generators/ax/service/base.py` & `optimas-0.6.0/optimas/generators/ax/service/base.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,37 +1,33 @@
 """Contains the definition of the base Ax generator using the service API."""
 
 from typing import List, Optional, Dict
 import os
 
 import torch
-from packaging import version
-from ax.version import version as ax_version
-from ax.core.observation import ObservationFeatures
+from ax.service.ax_client import AxClient
 from ax.service.utils.instantiation import (
     InstantiationBase,
     ObjectiveProperties,
+    FixedFeatures,
 )
 from ax.modelbridge.registry import Models
 from ax.modelbridge.generation_strategy import (
     GenerationStep,
     GenerationStrategy,
 )
 
-from optimas.utils.other import update_object
 from optimas.core import (
     Objective,
     Trial,
     VaryingParameter,
     Parameter,
     TrialStatus,
 )
 from optimas.generators.ax.base import AxGenerator
-from optimas.generators.base import Generator
-from .custom_ax import CustomAxClient as AxClient
 
 
 class AxServiceGenerator(AxGenerator):
     """Base class for all Ax generators using the service API.
 
     Parameters
     ----------
@@ -127,23 +123,17 @@
         self._parameter_constraints = parameter_constraints
         self._outcome_constraints = outcome_constraints
         self._ax_client = self._create_ax_client()
 
     def _ask(self, trials: List[Trial]) -> List[Trial]:
         """Fill in the parameter values of the requested trials."""
         for trial in trials:
-            try:
-                parameters, trial_id = self._ax_client.get_next_trial(
-                    fixed_features=self._fixed_features
-                )
-            # Occurs when not using a CustomAxClient (i.e., when the AxClient
-            # is provided by the user using an AxClientGenerator). In that
-            # case, there is also no need to support FixedFeatures.
-            except TypeError:
-                parameters, trial_id = self._ax_client.get_next_trial()
+            parameters, trial_id = self._ax_client.get_next_trial(
+                fixed_features=self._fixed_features
+            )
             trial.parameter_values = [
                 parameters.get(var.name) for var in self._varying_parameters
             ]
             trial.ax_trial_id = trial_id
         return trials
 
     def _tell(self, trials: List[Trial]) -> None:
@@ -167,17 +157,15 @@
                     trial.status != TrialStatus.FAILED
                     and not self._enforce_n_init
                 ):
                     generation_strategy = self._ax_client.generation_strategy
                     current_step = generation_strategy.current_step
                     # Reduce only if there are still Sobol trials left.
                     if current_step.model == Models.SOBOL:
-                        current_step.num_trials -= 1
-                        if version.parse(ax_version) >= version.parse("0.3.5"):
-                            current_step.transition_criteria[0].threshold -= 1
+                        current_step.transition_criteria[0].threshold -= 1
                         generation_strategy._maybe_move_to_next_step()
             finally:
                 if trial.completed:
                     outcome_evals = {}
                     # Add objective evaluations.
                     for ev in trial.objective_evaluations:
                         outcome_evals[ev.parameter.name] = (ev.value, ev.sem)
@@ -236,15 +224,15 @@
                     "target_value": var.fidelity_target_value,
                     "value_type": var.dtype.__name__,
                 }
             )
             if var.is_fixed:
                 fixed_parameters[var.name] = var.default_value
         # Store fixed parameters as fixed features.
-        self._fixed_features = ObservationFeatures(fixed_parameters)
+        self._fixed_features = FixedFeatures(fixed_parameters)
         return parameters
 
     def _create_ax_objectives(self) -> Dict[str, ObjectiveProperties]:
         """Create list of objectives to pass to an Ax."""
         objectives = {}
         for obj in self.objectives:
             objectives[obj.name] = ObjectiveProperties(minimize=obj.minimize)
@@ -262,46 +250,22 @@
             self._model_history_dir,
             "ax_client_at_eval_{}.json".format(
                 self._n_evaluated_trials_last_saved
             ),
         )
         self._ax_client.save_to_json_file(file_path)
 
-    def _prepare_to_send(self) -> None:
-        """Prepare generator to send to another process.
-
-        Delete the fitted model from the generation strategy. It can contain
-        pytorch tensors that prevent serialization.
-        """
+    def _update_parameter(self, parameter):
+        """Update a parameter from the search space."""
+        # Delete the fitted model from the generation strategy, otherwise
+        # the parameter won't be updated.
         generation_strategy = self._ax_client.generation_strategy
         if generation_strategy._model is not None:
             del generation_strategy._curr.model_spec._fitted_model
-            generation_strategy._curr.model_spec._fitted_model = None
-            del generation_strategy._model
-            generation_strategy._model = None
-
-    def _update(self, new_generator: Generator) -> None:
-        """Update generator with the attributes of a newer one.
-
-        This method is overrides the base one to make sure that the original
-        AxClient is updated and not simply replaced.
-
-        Parameters
-        ----------
-        new_generator : Generator
-            The newer version of the generator returned in ``persis_info``.
-
-        """
-        original_ax_client = self._ax_client
-        super()._update(new_generator)
-        update_object(original_ax_client, new_generator._ax_client)
-        self._ax_client = original_ax_client
-
-    def _update_parameter(self, parameter):
-        """Update a parameter from the search space."""
+        # Update parameter.
         parameters = self._create_ax_parameters()
         new_search_space = InstantiationBase.make_search_space(parameters, None)
         self._ax_client.experiment.search_space.update_parameter(
             new_search_space.parameters[parameter.name]
         )
 
     def _mark_trial_as_failed(self, trial: Trial):
```

### Comparing `optimas-0.5.0/optimas/generators/ax/service/multi_fidelity.py` & `optimas-0.6.0/optimas/generators/ax/service/multi_fidelity.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 """Contains the definition of the multi-fidelity Ax generator."""
 
 from typing import List, Optional, Dict
 
+from botorch.acquisition.knowledge_gradient import (
+    qMultiFidelityKnowledgeGradient,
+)
+from ax.utils.common.constants import Keys
 from ax.modelbridge.generation_strategy import GenerationStep
 from ax.modelbridge.registry import Models
 
 from optimas.core import Objective, VaryingParameter, Parameter
 from .base import AxServiceGenerator
 
 
@@ -102,28 +106,35 @@
             model_history_dir=model_history_dir,
         )
 
     def _create_generation_steps(
         self, bo_model_kwargs: Dict
     ) -> List[GenerationStep]:
         """Create generation steps for multifidelity optimization."""
-        # Add cost intercept to model kwargs.
-        bo_model_kwargs["cost_intercept"] = self.fidel_cost_intercept
+        # Add acquisition function to model kwargs.
+        bo_model_kwargs["botorch_acqf_class"] = qMultiFidelityKnowledgeGradient
 
         # Make generation strategy.
         steps = []
 
         # Add Sobol initialization with `n_init` random trials.
         steps.append(
             GenerationStep(model=Models.SOBOL, num_trials=self._n_init)
         )
 
         # Continue indefinitely with GPKG.
         steps.append(
             GenerationStep(
-                model=Models.GPKG,
+                model=Models.BOTORCH_MODULAR,
                 num_trials=-1,
                 model_kwargs=bo_model_kwargs,
-            )
+                model_gen_kwargs={
+                    "model_gen_options": {
+                        Keys.ACQF_KWARGS: {
+                            Keys.COST_INTERCEPT: self.fidel_cost_intercept
+                        }
+                    }
+                },
+            ),
         )
 
         return steps
```

### Comparing `optimas-0.5.0/optimas/generators/ax/service/single_fidelity.py` & `optimas-0.6.0/optimas/generators/ax/service/single_fidelity.py`

 * *Files identical despite different names*

### Comparing `optimas-0.5.0/optimas/generators/base.py` & `optimas-0.6.0/optimas/generators/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from copy import deepcopy
 from typing import List, Dict, Optional, Union
 
 import numpy as np
 import pandas as pd
 
 from optimas.utils.logger import get_logger
-from optimas.utils.other import update_object, convert_to_dataframe
+from optimas.utils.other import convert_to_dataframe
 from optimas.gen_functions import persistent_generator
 from optimas.core import (
     Objective,
     Trial,
     Evaluation,
     VaryingParameter,
     Parameter,
@@ -521,15 +521,14 @@
         run_params : dict
             Dictionary containing the number of processes and gpus
             required.
         max_evals : int
             Maximum number of evaluations to generate.
 
         """
-        self._prepare_to_send()
         gen_specs = {
             # Generator function.
             "gen_f": self._gen_function,
             # Generator input. This is a RNG, no need for inputs.
             "in": ["sim_id"],
             "persis_in": (
                 ["sim_id", "trial_index", "trial_status"]
@@ -563,58 +562,26 @@
         return gen_specs
 
     def get_libe_specs(self) -> Dict:
         """Get the libEnsemble libe_specs."""
         libE_specs = {}
         return libE_specs
 
-    def _prepare_to_send(self) -> None:
-        """Prepare generator to send to another process.
-
-        This method is necessary because the generator, when given to
-        libEnsemble, is sent to another process (the process of the generator
-        worker) and then sent back to optimas at the end of the run. In order
-        for it to be sent, the generator must be serialized, and sometimes
-        some of the contents of the generator cannot be serialized. The
-        purpose of this method is to take care of the attributes that prevent
-        serialization, and is always called before the generator is sent
-        to/from libEnsemble.
-
-        It must be implemented by the subclasses, if needed.
-        """
-        pass
-
-    def _update(self, new_generator: Generator) -> None:
-        """Update generator with the attributes of a newer one.
-
-        This method is only intended to be used internally by an
-        ``Exploration`` after a run is completed. It is needed because the
-        ``Generator`` given to ``libEnsemble`` is passed as a copy to the
-        generator worker and is therefore not updated during the run.
-
-        Parameters
-        ----------
-        new_generator : Generator
-            The newer version of the generator returned in ``persis_info``.
-
-        """
-        update_object(self, new_generator)
-
     def _ask(self, trials: List[Trial]) -> List[Trial]:
         """Ask method to be implemented by the Generator subclasses.
 
         Parameters
         ----------
         trials : list of Trial
             A list with as many trials as requested to the generator. The
             trials do not yet contain the values of the varying parameters.
             These values should instead be supplied in this method.
 
         """
-        pass
+        return trials
 
     def _tell(self, trials: List[Trial]) -> None:
         """Tell method to be implemented by the Generator subclasses.
 
         Parameters
         ----------
         trials : list of Trial
```

### Comparing `optimas-0.5.0/optimas/generators/grid_sampling.py` & `optimas-0.6.0/optimas/generators/grid_sampling.py`

 * *Files identical despite different names*

### Comparing `optimas-0.5.0/optimas/generators/line_sampling.py` & `optimas-0.6.0/optimas/generators/line_sampling.py`

 * *Files identical despite different names*

### Comparing `optimas-0.5.0/optimas/generators/random_sampling.py` & `optimas-0.6.0/optimas/generators/random_sampling.py`

 * *Files identical despite different names*

### Comparing `optimas-0.5.0/optimas/sim_functions.py` & `optimas-0.6.0/optimas/sim_functions.py`

 * *Files identical despite different names*

### Comparing `optimas-0.5.0/optimas/utils/logger.py` & `optimas-0.6.0/optimas/utils/logger.py`

 * *Files identical despite different names*

### Comparing `optimas-0.5.0/optimas/utils/other.py` & `optimas-0.6.0/optimas/utils/other.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,34 +1,15 @@
 """Definition of other utilities used internally by optimas."""
 
-from typing import Any, Union, List, Dict
+from typing import Union, List, Dict
 
 import numpy as np
 import pandas as pd
 
 
-def update_object(object_old: Any, object_new: Any) -> None:
-    """Update the attributes of an object with those from a newer one.
-
-    This method is intended to be used with objects of the same type and that
-    have a `__dict__` attribute.
-
-    Parameters
-    ----------
-    object_old : Any
-        The object to be updated.
-    object_new : Any
-        The object from which to get the updated attributes.
-
-    """
-    assert isinstance(object_new, type(object_old)), "Object types don't match"
-    for key, value in vars(object_new).items():
-        setattr(object_old, key, value)
-
-
 def convert_to_dataframe(
     data: Union[Dict, List[Dict], np.ndarray, pd.DataFrame]
 ) -> pd.DataFrame:
     """Convert input data to a pandas DataFrame.
 
     Parameters
     ----------
```

### Comparing `optimas-0.5.0/optimas.egg-info/PKG-INFO` & `optimas-0.6.0/optimas.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,36 +1,35 @@
 Metadata-Version: 2.1
 Name: optimas
-Version: 0.5.0
+Version: 0.6.0
 Summary: Optimization at scale, powered by libEnsemble
 Author-email: Optimas Developers <angel.ferran.pousa@desy.de>
 License: BSD-3-Clause-LBNL
 Project-URL: Documentation, https://optimas.readthedocs.io/
 Keywords: optimization,scale,bayesian
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.9
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
-Requires-Dist: libensemble>=1.2
+Requires-Dist: libensemble>=1.3.0
 Requires-Dist: jinja2
 Requires-Dist: pandas
 Requires-Dist: mpi4py
 Requires-Dist: pydantic>=2.0
 Provides-Extra: test
 Requires-Dist: flake8; extra == "test"
 Requires-Dist: pytest; extra == "test"
-Requires-Dist: ax-platform>=0.3.4; extra == "test"
+Requires-Dist: ax-platform>=0.4.0; extra == "test"
 Requires-Dist: matplotlib; extra == "test"
 Provides-Extra: all
-Requires-Dist: ax-platform>=0.3.4; extra == "all"
+Requires-Dist: ax-platform>=0.4.0; extra == "all"
 
 [![PyPI](https://img.shields.io/pypi/v/optimas)](https://pypi.org/project/optimas/)
 [![Conda Version](https://img.shields.io/conda/vn/conda-forge/optimas.svg)](https://anaconda.org/conda-forge/optimas)
 [![tests badge](https://github.com/optimas-org/optimas/actions/workflows/unix.yml/badge.svg)](https://github.com/optimas-org/optimas/actions)
 [![Documentation Status](https://readthedocs.org/projects/optimas/badge/?version=latest)](https://optimas.readthedocs.io/en/latest/?badge=latest)
 [![DOI](https://zenodo.org/badge/287560975.svg)](https://zenodo.org/badge/latestdoi/287560975)
 [![License](https://img.shields.io/pypi/l/optimas.svg)](license.txt)
@@ -78,15 +77,15 @@
 ```sh
 conda install optimas --channel conda-forge
 ```
 or directly from GitHub:
 ```sh
 pip install git+https://github.com/optimas-org/optimas.git
 ```
-Make sure `mpi4py` is available in your environment before installing optimas. Fore more details, check out the full [installation guide](https://optimas.readthedocs.io/en/latest/user_guide/installation_local.html). We have also prepared dedicated installation instructions for some HPC systems such as
+Make sure `mpi4py` is available in your environment before installing optimas. For more details, check out the full [installation guide](https://optimas.readthedocs.io/en/latest/user_guide/installation_local.html). We have also prepared dedicated installation instructions for some HPC systems such as
 [JUWELS (JSC)](https://optimas.readthedocs.io/en/latest/user_guide/installation_juwels.html),
 [Maxwell (DESY)](https://optimas.readthedocs.io/en/latest/user_guide/installation_maxwell.html) and
 [Perlmutter (NERSC)](https://optimas.readthedocs.io/en/latest/user_guide/installation_perlmutter.html).
 
 
 ## Documentation
 For more information on how to use Optimas, check out the [documentation](https://optimas.readthedocs.io/). You'll find installation instructions, a user guide, [examples](https://optimas.readthedocs.io/en/latest/examples/index.html) and the API reference.
```

#### html2text {}

```diff
@@ -1,31 +1,30 @@
-Metadata-Version: 2.1 Name: optimas Version: 0.5.0 Summary: Optimization at
+Metadata-Version: 2.1 Name: optimas Version: 0.6.0 Summary: Optimization at
 scale, powered by libEnsemble Author-email: Optimas Developers
 desy.de> License: BSD-3-Clause-LBNL Project-URL: Documentation, https://
 optimas.readthedocs.io/ Keywords: optimization,scale,bayesian Classifier:
 Development Status :: 3 - Alpha Classifier: Intended Audience :: Science/
 Research Classifier: Topic :: Scientific/Engineering Classifier: Operating
-System :: OS Independent Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
-Language :: Python :: 3.11 Requires-Python: >=3.9 Description-Content-Type:
-text/markdown Requires-Dist: libensemble>=1.2 Requires-Dist: jinja2 Requires-
-Dist: pandas Requires-Dist: mpi4py Requires-Dist: pydantic>=2.0 Provides-Extra:
-test Requires-Dist: flake8; extra == "test" Requires-Dist: pytest; extra ==
-"test" Requires-Dist: ax-platform>=0.3.4; extra == "test" Requires-Dist:
-matplotlib; extra == "test" Provides-Extra: all Requires-Dist: ax-
-platform>=0.3.4; extra == "all" [![PyPI](https://img.shields.io/pypi/v/
-optimas)](https://pypi.org/project/optimas/) [![Conda Version](https://
-img.shields.io/conda/vn/conda-forge/optimas.svg)](https://anaconda.org/conda-
-forge/optimas) [![tests badge](https://github.com/optimas-org/optimas/actions/
-workflows/unix.yml/badge.svg)](https://github.com/optimas-org/optimas/actions)
-[![Documentation Status](https://readthedocs.org/projects/optimas/badge/
-?version=latest)](https://optimas.readthedocs.io/en/latest/?badge=latest) [!
-[DOI](https://zenodo.org/badge/287560975.svg)](https://zenodo.org/badge/
-latestdoi/287560975) [![License](https://img.shields.io/pypi/l/optimas.svg)]
-(license.txt)
+System :: OS Independent Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11 Requires-Python: >=3.10
+Description-Content-Type: text/markdown Requires-Dist: libensemble>=1.3.0
+Requires-Dist: jinja2 Requires-Dist: pandas Requires-Dist: mpi4py Requires-
+Dist: pydantic>=2.0 Provides-Extra: test Requires-Dist: flake8; extra == "test"
+Requires-Dist: pytest; extra == "test" Requires-Dist: ax-platform>=0.4.0; extra
+== "test" Requires-Dist: matplotlib; extra == "test" Provides-Extra: all
+Requires-Dist: ax-platform>=0.4.0; extra == "all" [![PyPI](https://
+img.shields.io/pypi/v/optimas)](https://pypi.org/project/optimas/) [![Conda
+Version](https://img.shields.io/conda/vn/conda-forge/optimas.svg)](https://
+anaconda.org/conda-forge/optimas) [![tests badge](https://github.com/optimas-
+org/optimas/actions/workflows/unix.yml/badge.svg)](https://github.com/optimas-
+org/optimas/actions) [![Documentation Status](https://readthedocs.org/projects/
+optimas/badge/?version=latest)](https://optimas.readthedocs.io/en/latest/
+?badge=latest) [![DOI](https://zenodo.org/badge/287560975.svg)](https://
+zenodo.org/badge/latestdoi/287560975) [![License](https://img.shields.io/pypi/
+l/optimas.svg)](license.txt)
                                 _[_o_p_t_i_m_a_s_ _l_o_g_o_]
             ******** OOppttiimmiizzaattiioonn aatt ssccaallee,, ppoowweerreedd bbyy _ll_ii_bb_EE_nn_ss_ee_mm_bb_ll_ee ********
                              _EE_xx_pp_ll_oo_rr_ee_ _tt_hh_ee_ _dd_oo_cc_ss_ _?Â_?»
 
                    _V_i_e_w_ _E_x_a_m_p_l_e_s Â· _S_u_p_p_o_r_t Â· _A_P_I_ _R_e_f_e_r_e_n_c_e
 Optimas is a Python library designed for highly scalable optimization, from
 laptops to massively-parallel supercomputers. ## Key Features -
@@ -38,15 +37,15 @@
 **Advanced Optimization**: Optimas integrates algorithms from the [Ax](https://
 github.com/facebook/Ax) library, offering both single- and multi-objective
 Bayesian optimization. This includes advanced techniques such as multi-fidelity
 and multi-task algorithms. ## Installation You can install Optimas from PyPI
 (recommended): ```sh pip install optimas ``` from conda-forge: ```sh conda
 install optimas --channel conda-forge ``` or directly from GitHub: ```sh pip
 install git+https://github.com/optimas-org/optimas.git ``` Make sure `mpi4py`
-is available in your environment before installing optimas. Fore more details,
+is available in your environment before installing optimas. For more details,
 check out the full [installation guide](https://optimas.readthedocs.io/en/
 latest/user_guide/installation_local.html). We have also prepared dedicated
 installation instructions for some HPC systems such as [JUWELS (JSC)](https://
 optimas.readthedocs.io/en/latest/user_guide/installation_juwels.html), [Maxwell
 (DESY)](https://optimas.readthedocs.io/en/latest/user_guide/
 installation_maxwell.html) and [Perlmutter (NERSC)](https://
 optimas.readthedocs.io/en/latest/user_guide/installation_perlmutter.html). ##
```

### Comparing `optimas-0.5.0/optimas.egg-info/SOURCES.txt` & `optimas-0.6.0/optimas.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -35,27 +35,27 @@
 optimas/generators/ax/import_error_dummy_generator.py
 optimas/generators/ax/developer/__init__.py
 optimas/generators/ax/developer/ax_metric.py
 optimas/generators/ax/developer/multitask.py
 optimas/generators/ax/service/__init__.py
 optimas/generators/ax/service/ax_client.py
 optimas/generators/ax/service/base.py
-optimas/generators/ax/service/custom_ax.py
 optimas/generators/ax/service/multi_fidelity.py
 optimas/generators/ax/service/single_fidelity.py
 optimas/utils/__init__.py
 optimas/utils/logger.py
 optimas/utils/other.py
 tests/test_analyzed_parameters.py
 tests/test_ax_generators.py
 tests/test_ax_model_manager.py
 tests/test_chain_evaluator.py
 tests/test_comms.py
 tests/test_env_script.py
 tests/test_exploration_diagnostics.py
 tests/test_exploration_resume.py
 tests/test_function_evaluator.py
+tests/test_gpu_resources.py
 tests/test_grid_sampling.py
 tests/test_line_sampling.py
 tests/test_manual_exploration.py
 tests/test_random_sampling.py
 tests/test_template_evaluator.py
```

### Comparing `optimas-0.5.0/pyproject.toml` & `optimas-0.6.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -5,44 +5,43 @@
 [project]
 name = 'optimas'
 description = 'Optimization at scale, powered by libEnsemble'
 authors = [
     {name = 'Optimas Developers', email = 'angel.ferran.pousa@desy.de'},
 ]
 readme = 'README.md'
-requires-python = '>=3.9'
+requires-python = '>=3.10'
 keywords = ['optimization', 'scale', 'bayesian']
 license = {text = 'BSD-3-Clause-LBNL'}
 classifiers = [
     'Development Status :: 3 - Alpha',
     'Intended Audience :: Science/Research',
     'Topic :: Scientific/Engineering',
     'Operating System :: OS Independent',
-    'Programming Language :: Python :: 3.9',
     'Programming Language :: Python :: 3.10',
     'Programming Language :: Python :: 3.11',
 ]
 dependencies = [
-    'libensemble >= 1.2',
+    'libensemble >= 1.3.0',
     'jinja2',
     'pandas',
     'mpi4py',
     'pydantic >= 2.0',
 ]
 dynamic = ['version']
 
 [project.optional-dependencies]
 test = [
     'flake8',
     'pytest',
-    'ax-platform >= 0.3.4',
+    'ax-platform >= 0.4.0',
     'matplotlib',
 ]
 all = [
-    'ax-platform >= 0.3.4',
+    'ax-platform >= 0.4.0',
 ]
 
 [project.urls]
 Documentation = 'https://optimas.readthedocs.io/'
 
 [tool.setuptools.dynamic]
 version = {attr = "optimas.__version__"}
```

### Comparing `optimas-0.5.0/tests/test_analyzed_parameters.py` & `optimas-0.6.0/tests/test_analyzed_parameters.py`

 * *Files identical despite different names*

### Comparing `optimas-0.5.0/tests/test_ax_generators.py` & `optimas-0.6.0/tests/test_ax_generators.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import os
 import threading
 
 import numpy as np
 from ax.service.ax_client import AxClient, ObjectiveProperties
 from ax.utils.measurement.synthetic_functions import hartmann6
 
 from optimas.explorations import Exploration
@@ -343,15 +344,15 @@
     # Perform checks.
     check_run_ax_service(ax_client, gen, exploration, len(trials_to_fail))
 
 
 def test_ax_single_fidelity_updated_params():
     """
     Test that an exploration with a single-fidelity generator runs
-    as expected when the varing parameters are updated.
+    as expected when the varying parameters are updated.
     """
     # Prevent trials from failing in this test.
     global trial_count
     global trials_to_fail
     trial_count = 0
     trials_to_fail = []
 
@@ -725,14 +726,25 @@
         df = ax_client.get_trials_data_frame()
         for j in range(i):
             assert df["generation_method"][j] == "Manual"
         for k in range(i, n_init - 1):
             assert df["generation_method"][k] == "Sobol"
         df["generation_method"][min(i, n_init)] == "GPEI"
 
+    # Try to load saved client from json. This used to fail when the SOBOL
+    # step was skipped due to n_external > n_init. It is added here to prevent
+    # the issue from coming back.
+    AxClient.load_from_json_file(
+        filepath=os.path.join(
+            exploration.exploration_dir_path,
+            "model_history",
+            "ax_client_at_eval_5.json",
+        )
+    )
+
     # Test single case with `enforce_n_init=True`
     gen = AxSingleFidelityGenerator(
         varying_parameters=[var1, var2],
         objectives=[obj],
         n_init=n_init,
         enforce_n_init=True,
     )
```

### Comparing `optimas-0.5.0/tests/test_ax_model_manager.py` & `optimas-0.6.0/tests/test_ax_model_manager.py`

 * *Files identical despite different names*

### Comparing `optimas-0.5.0/tests/test_chain_evaluator.py` & `optimas-0.6.0/tests/test_chain_evaluator.py`

 * *Files identical despite different names*

### Comparing `optimas-0.5.0/tests/test_comms.py` & `optimas-0.6.0/tests/test_comms.py`

 * *Files identical despite different names*

### Comparing `optimas-0.5.0/tests/test_env_script.py` & `optimas-0.6.0/tests/test_env_script.py`

 * *Files identical despite different names*

### Comparing `optimas-0.5.0/tests/test_exploration_diagnostics.py` & `optimas-0.6.0/tests/test_exploration_diagnostics.py`

 * *Files identical despite different names*

### Comparing `optimas-0.5.0/tests/test_exploration_resume.py` & `optimas-0.6.0/tests/test_exploration_resume.py`

 * *Files identical despite different names*

### Comparing `optimas-0.5.0/tests/test_function_evaluator.py` & `optimas-0.6.0/tests/test_function_evaluator.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,74 +1,97 @@
 import os
 
 import numpy as np
 import matplotlib.pyplot as plt
+import pytest
 
 from optimas.explorations import Exploration
 from optimas.generators import RandomSamplingGenerator
 from optimas.evaluators import FunctionEvaluator
 from optimas.core import VaryingParameter, Objective, Parameter
+from optimas.diagnostics import ExplorationDiagnostics
 
 
 def eval_func(input_params, output_params):
     """Evaluation function used for testing"""
     x0 = input_params["x0"]
     x1 = input_params["x1"]
     result = -(x0 + 10 * np.cos(x0)) * (x1 + 5 * np.cos(x1))
     output_params["f"] = result
     output_params["p0"] = np.array([[1, 2, 3, 4], [2, 6, 7, 4]])
     output_params["p1"] = np.array([[1, 2, 3, 4], [2, 6, 7, 4]])
     plt.figure()
     plt.plot(output_params["p1"][0], output_params["p1"][1])
     output_params["fig"] = plt.gcf()
+    plt.savefig("fig.png")
 
 
 def test_function_evaluator():
     """Test that an exploration runs successfully with a function evaluator."""
-    # Define variables and objectives.
-    var1 = VaryingParameter("x0", -50.0, 5.0)
-    var2 = VaryingParameter("x1", -5.0, 15.0)
-    obj = Objective("f", minimize=False)
-    # Test also more complex analyzed parameters.
-    p0 = Parameter("p0", dtype=(float, (2, 4)))
-    p1 = Parameter("p1", dtype="O")
-    p2 = Parameter("fig", dtype="O")
-
-    # Create generator.
-    gen = RandomSamplingGenerator(
-        varying_parameters=[var1, var2],
-        objectives=[obj],
-        analyzed_parameters=[p0, p1, p2],
-    )
-
-    # Create function evaluator.
-    ev = FunctionEvaluator(function=eval_func)
-
-    # Create exploration.
-    exploration = Exploration(
-        generator=gen,
-        evaluator=ev,
-        max_evals=10,
-        sim_workers=2,
-        exploration_dir_path="./tests_output/test_function_evaluator",
-    )
-
-    # Run exploration.
-    exploration.run()
-
-    # Check that the multidimensional analyzed parameters worked as expected.
-    for p0_data in exploration.history["p0"]:
-        np.testing.assert_array_equal(
-            np.array(p0_data), np.array([[1, 2, 3, 4], [2, 6, 7, 4]])
+
+    create_dirs_options = [False, True]
+
+    for create_dirs in create_dirs_options:
+        # Define variables and objectives.
+        var1 = VaryingParameter("x0", -50.0, 5.0)
+        var2 = VaryingParameter("x1", -5.0, 15.0)
+        obj = Objective("f", minimize=False)
+        # Test also more complex analyzed parameters.
+        p0 = Parameter("p0", dtype=(float, (2, 4)))
+        p1 = Parameter("p1", dtype="O")
+        p2 = Parameter("fig", dtype="O")
+
+        # Create generator.
+        gen = RandomSamplingGenerator(
+            varying_parameters=[var1, var2],
+            objectives=[obj],
+            analyzed_parameters=[p0, p1, p2],
         )
-    for p1_data in exploration.history["p1"]:
-        np.testing.assert_array_equal(
-            np.array(p1_data), np.array([[1, 2, 3, 4], [2, 6, 7, 4]])
+
+        # Create function evaluator.
+        ev = FunctionEvaluator(
+            function=eval_func, create_evaluation_dirs=create_dirs
         )
-    for i, fig in enumerate(exploration.history["fig"]):
-        fig.savefig(
-            os.path.join(exploration.exploration_dir_path, f"test_fig_{i}.png")
+
+        # Create exploration.
+        exploration = Exploration(
+            generator=gen,
+            evaluator=ev,
+            max_evals=10,
+            sim_workers=2,
+            exploration_dir_path="./tests_output/test_function_evaluator",
         )
 
+        # Run exploration.
+        exploration.run()
+
+        # Check that the multidimensional analyzed parameters worked as expected.
+        for p0_data in exploration.history["p0"]:
+            np.testing.assert_array_equal(
+                np.array(p0_data), np.array([[1, 2, 3, 4], [2, 6, 7, 4]])
+            )
+        for p1_data in exploration.history["p1"]:
+            np.testing.assert_array_equal(
+                np.array(p1_data), np.array([[1, 2, 3, 4], [2, 6, 7, 4]])
+            )
+        for i, fig in enumerate(exploration.history["fig"]):
+            fig.savefig(
+                os.path.join(
+                    exploration.exploration_dir_path, f"test_fig_{i}.png"
+                )
+            )
+
+        diags = ExplorationDiagnostics(exploration)
+        for trial_index in diags.history.trial_index:
+            # Check that evaluation folders were created and the data was
+            # stored in them.
+            if create_dirs:
+                trial_dir = diags.get_evaluation_dir_path(trial_index)
+                assert os.path.exists(os.path.join(trial_dir, "fig.png"))
+            # Make sure no folders were created.
+            else:
+                with pytest.raises(ValueError):
+                    diags.get_evaluation_dir_path(trial_index)
+
 
 if __name__ == "__main__":
     test_function_evaluator()
```

### Comparing `optimas-0.5.0/tests/test_grid_sampling.py` & `optimas-0.6.0/tests/test_grid_sampling.py`

 * *Files identical despite different names*

### Comparing `optimas-0.5.0/tests/test_line_sampling.py` & `optimas-0.6.0/tests/test_line_sampling.py`

 * *Files identical despite different names*

### Comparing `optimas-0.5.0/tests/test_manual_exploration.py` & `optimas-0.6.0/tests/test_manual_exploration.py`

 * *Files identical despite different names*

### Comparing `optimas-0.5.0/tests/test_random_sampling.py` & `optimas-0.6.0/tests/test_random_sampling.py`

 * *Files identical despite different names*

### Comparing `optimas-0.5.0/tests/test_template_evaluator.py` & `optimas-0.6.0/tests/test_template_evaluator.py`

 * *Files identical despite different names*

