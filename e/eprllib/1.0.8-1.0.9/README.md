# Comparing `tmp/eprllib-1.0.8.tar.gz` & `tmp/eprllib-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eprllib-1.0.8.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "eprllib-1.0.9.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `eprllib-1.0.8.tar` & `eprllib-1.0.9.tar`

### file list

```diff
@@ -1,36 +1,41 @@
--rw-r--r--   0        0        0     6706 2024-03-22 12:29:57.414473 eprllib-1.0.8/README.md
--rw-r--r--   0        0        0      661 2024-03-28 14:18:44.367713 eprllib-1.0.8/pyproject.toml
--rw-r--r--   0        0        0        0 2024-02-23 13:27:42.113993 eprllib-1.0.8/src/eprllib/__init__.py
--rw-r--r--   0        0        0        0 2024-02-12 10:07:03.001250 eprllib-1.0.8/src/eprllib/agents/__init__.py
--rw-r--r--   0        0        0     5449 2024-03-14 16:24:23.397736 eprllib-1.0.8/src/eprllib/agents/conventional.py
--rw-r--r--   0        0        0     1028 2024-03-21 08:40:43.671486 eprllib-1.0.8/src/eprllib/agents/holon_config.py
--rw-r--r--   0        0        0     1008 2024-02-12 10:25:28.186353 eprllib-1.0.8/src/eprllib/agents/user.py
--rw-r--r--   0        0        0        2 2024-02-23 13:31:03.360381 eprllib-1.0.8/src/eprllib/env/__init__.py
--rw-r--r--   0        0        0        0 2024-03-21 19:16:29.819874 eprllib-1.0.8/src/eprllib/env/multiagent/__init__.py
--rw-r--r--   0        0        0     7553 2024-03-28 10:22:08.162993 eprllib-1.0.8/src/eprllib/env/multiagent/marl_ep_gym_env.py
--rw-r--r--   0        0        0    24709 2024-03-28 14:20:12.744895 eprllib-1.0.8/src/eprllib/env/multiagent/marl_ep_runner.py
--rw-r--r--   0        0        0     7670 2024-03-21 15:31:48.407127 eprllib-1.0.8/src/eprllib/env/simpleagent/VENT_ep_gym_env.py
--rw-r--r--   0        0        0    20698 2024-03-21 15:31:48.407127 eprllib-1.0.8/src/eprllib/env/simpleagent/VENT_ep_runner.py
--rw-r--r--   0        0        0        0 2024-03-21 19:16:52.042116 eprllib-1.0.8/src/eprllib/env/simpleagent/__init__.py
--rw-r--r--   0        0        0     6060 2024-03-21 15:31:48.402974 eprllib-1.0.8/src/eprllib/postprocess/VENT_init_conventional.py
--rw-r--r--   0        0        0     6064 2024-03-21 15:31:48.402974 eprllib-1.0.8/src/eprllib/postprocess/VENT_init_conventional_test.py
--rw-r--r--   0        0        0     5500 2024-03-21 15:31:48.401949 eprllib-1.0.8/src/eprllib/postprocess/VENT_init_evaluation.py
--rw-r--r--   0        0        0        2 2024-02-23 13:31:03.369889 eprllib-1.0.8/src/eprllib/postprocess/__init__.py
--rw-r--r--   0        0        0     6465 2024-03-21 15:31:48.407127 eprllib-1.0.8/src/eprllib/postprocess/marl_init_conventional.py
--rw-r--r--   0        0        0     6083 2024-03-21 15:31:48.407127 eprllib-1.0.8/src/eprllib/postprocess/marl_init_evaluation.py
--rw-r--r--   0        0        0     6063 2024-03-21 15:31:48.402974 eprllib-1.0.8/src/eprllib/postprocess/marl_init_noventilation.py
--rw-r--r--   0        0        0   450806 2024-03-21 08:51:31.613528 eprllib-1.0.8/src/eprllib/postprocess/marl_results_evaluation.ipynb
--rw-r--r--   0        0        0     3002 2024-02-22 11:24:29.811391 eprllib-1.0.8/src/eprllib/postprocess/neural_networ_analysis.ipynb
--rw-r--r--   0        0        0   937103 2024-03-21 08:40:43.872034 eprllib-1.0.8/src/eprllib/postprocess/results_evaluation.ipynb
--rw-r--r--   0        0        0   982932 2024-03-21 08:40:43.887790 eprllib-1.0.8/src/eprllib/postprocess/results_evaluation_test.ipynb
--rw-r--r--   0        0        0   909856 2024-03-21 08:40:43.907284 eprllib-1.0.8/src/eprllib/postprocess/test_results_evaluation.ipynb
--rw-r--r--   0        0        0        2 2024-02-23 13:31:03.372239 eprllib-1.0.8/src/eprllib/preprocess/__init__.py
--rw-r--r--   0        0        0     5797 2024-03-21 15:31:48.398206 eprllib-1.0.8/src/eprllib/preprocess/conventional_experience.py
--rw-r--r--   0        0        0        0 2024-02-12 10:39:26.603572 eprllib-1.0.8/src/eprllib/tools/__init__.py
--rw-r--r--   0        0        0      829 2024-03-28 10:22:08.162993 eprllib-1.0.8/src/eprllib/tools/action_transformers.py
--rw-r--r--   0        0        0     1402 2024-02-24 11:12:25.969964 eprllib-1.0.8/src/eprllib/tools/devices_space_action.py
--rw-r--r--   0        0        0    19846 2024-03-21 15:31:48.398206 eprllib-1.0.8/src/eprllib/tools/ep_episode_config.py
--rw-r--r--   0        0        0     6170 2024-03-28 14:17:34.088567 eprllib-1.0.8/src/eprllib/tools/rewards.py
--rw-r--r--   0        0        0      445 2024-03-22 12:47:59.425198 eprllib-1.0.8/src/eprllib/tools/utils.py
--rw-r--r--   0        0        0     7134 2024-03-21 20:29:35.640440 eprllib-1.0.8/src/eprllib/tools/weather_utils.py
--rw-r--r--   0        0        0     7087 1970-01-01 00:00:00.000000 eprllib-1.0.8/PKG-INFO
+-rw-r--r--   0        0        0     6706 2024-03-22 12:29:57.414473 eprllib-1.0.9/README.md
+-rw-r--r--   0        0        0      661 2024-03-28 19:56:41.798422 eprllib-1.0.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-02-23 13:27:42.113993 eprllib-1.0.9/src/eprllib/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-12 10:07:03.001250 eprllib-1.0.9/src/eprllib/agents/__init__.py
+-rw-r--r--   0        0        0     5449 2024-03-14 16:24:23.397736 eprllib-1.0.9/src/eprllib/agents/conventional.py
+-rw-r--r--   0        0        0     1028 2024-03-21 08:40:43.671486 eprllib-1.0.9/src/eprllib/agents/holon_config.py
+-rw-r--r--   0        0        0     1008 2024-02-12 10:25:28.186353 eprllib-1.0.9/src/eprllib/agents/user.py
+-rw-r--r--   0        0        0        0 2024-03-28 19:41:05.994140 eprllib-1.0.9/src/eprllib/env/ExampleFiles/__init__.py
+-rw-r--r--   0        0        0  1648753 2023-09-29 02:24:12.463812 eprllib-1.0.9/src/eprllib/env/ExampleFiles/epw/USA_IL_Chicago-OHare.Intl.AP.725300_TMY3.epw
+-rw-r--r--   0        0        0        0 2024-03-28 19:44:21.356531 eprllib-1.0.9/src/eprllib/env/ExampleFiles/epw/__init__.py
+-rw-r--r--   0        0        0   245096 2024-03-28 19:55:28.762266 eprllib-1.0.9/src/eprllib/env/ExampleFiles/idf/RefBldgSmallOfficeNew2004_Chicago.idf
+-rw-r--r--   0        0        0        0 2024-03-28 19:44:14.625089 eprllib-1.0.9/src/eprllib/env/ExampleFiles/idf/__init__.py
+-rw-r--r--   0        0        0        2 2024-02-23 13:31:03.360381 eprllib-1.0.9/src/eprllib/env/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-21 19:16:29.819874 eprllib-1.0.9/src/eprllib/env/multiagent/__init__.py
+-rw-r--r--   0        0        0     7553 2024-03-28 10:22:08.162993 eprllib-1.0.9/src/eprllib/env/multiagent/marl_ep_gym_env.py
+-rw-r--r--   0        0        0    24709 2024-03-28 14:20:12.744895 eprllib-1.0.9/src/eprllib/env/multiagent/marl_ep_runner.py
+-rw-r--r--   0        0        0     7670 2024-03-21 15:31:48.407127 eprllib-1.0.9/src/eprllib/env/simpleagent/VENT_ep_gym_env.py
+-rw-r--r--   0        0        0    20698 2024-03-21 15:31:48.407127 eprllib-1.0.9/src/eprllib/env/simpleagent/VENT_ep_runner.py
+-rw-r--r--   0        0        0        0 2024-03-21 19:16:52.042116 eprllib-1.0.9/src/eprllib/env/simpleagent/__init__.py
+-rw-r--r--   0        0        0     6060 2024-03-21 15:31:48.402974 eprllib-1.0.9/src/eprllib/postprocess/VENT_init_conventional.py
+-rw-r--r--   0        0        0     6064 2024-03-21 15:31:48.402974 eprllib-1.0.9/src/eprllib/postprocess/VENT_init_conventional_test.py
+-rw-r--r--   0        0        0     5500 2024-03-21 15:31:48.401949 eprllib-1.0.9/src/eprllib/postprocess/VENT_init_evaluation.py
+-rw-r--r--   0        0        0        2 2024-02-23 13:31:03.369889 eprllib-1.0.9/src/eprllib/postprocess/__init__.py
+-rw-r--r--   0        0        0     6465 2024-03-21 15:31:48.407127 eprllib-1.0.9/src/eprllib/postprocess/marl_init_conventional.py
+-rw-r--r--   0        0        0     6083 2024-03-21 15:31:48.407127 eprllib-1.0.9/src/eprllib/postprocess/marl_init_evaluation.py
+-rw-r--r--   0        0        0     6063 2024-03-21 15:31:48.402974 eprllib-1.0.9/src/eprllib/postprocess/marl_init_noventilation.py
+-rw-r--r--   0        0        0   450806 2024-03-21 08:51:31.613528 eprllib-1.0.9/src/eprllib/postprocess/marl_results_evaluation.ipynb
+-rw-r--r--   0        0        0     3002 2024-02-22 11:24:29.811391 eprllib-1.0.9/src/eprllib/postprocess/neural_networ_analysis.ipynb
+-rw-r--r--   0        0        0   937103 2024-03-21 08:40:43.872034 eprllib-1.0.9/src/eprllib/postprocess/results_evaluation.ipynb
+-rw-r--r--   0        0        0   982932 2024-03-21 08:40:43.887790 eprllib-1.0.9/src/eprllib/postprocess/results_evaluation_test.ipynb
+-rw-r--r--   0        0        0   909856 2024-03-21 08:40:43.907284 eprllib-1.0.9/src/eprllib/postprocess/test_results_evaluation.ipynb
+-rw-r--r--   0        0        0        2 2024-02-23 13:31:03.372239 eprllib-1.0.9/src/eprllib/preprocess/__init__.py
+-rw-r--r--   0        0        0     5797 2024-03-21 15:31:48.398206 eprllib-1.0.9/src/eprllib/preprocess/conventional_experience.py
+-rw-r--r--   0        0        0        0 2024-02-12 10:39:26.603572 eprllib-1.0.9/src/eprllib/tools/__init__.py
+-rw-r--r--   0        0        0      829 2024-03-28 10:22:08.162993 eprllib-1.0.9/src/eprllib/tools/action_transformers.py
+-rw-r--r--   0        0        0     1402 2024-02-24 11:12:25.969964 eprllib-1.0.9/src/eprllib/tools/devices_space_action.py
+-rw-r--r--   0        0        0    19846 2024-03-21 15:31:48.398206 eprllib-1.0.9/src/eprllib/tools/ep_episode_config.py
+-rw-r--r--   0        0        0     6170 2024-03-28 14:17:34.088567 eprllib-1.0.9/src/eprllib/tools/rewards.py
+-rw-r--r--   0        0        0      445 2024-03-22 12:47:59.425198 eprllib-1.0.9/src/eprllib/tools/utils.py
+-rw-r--r--   0        0        0     7134 2024-03-21 20:29:35.640440 eprllib-1.0.9/src/eprllib/tools/weather_utils.py
+-rw-r--r--   0        0        0     7087 1970-01-01 00:00:00.000000 eprllib-1.0.9/PKG-INFO
```

### Comparing `eprllib-1.0.8/README.md` & `eprllib-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `eprllib-1.0.8/pyproject.toml` & `eprllib-1.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "eprllib"
-version = "1.0.8"
+version = "1.0.9"
 authors = [
   { name="Germán Rodolfo Henderson"},
 ]
 description = "Building control trought DRL."
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `eprllib-1.0.8/src/eprllib/agents/conventional.py` & `eprllib-1.0.9/src/eprllib/agents/conventional.py`

 * *Files identical despite different names*

### Comparing `eprllib-1.0.8/src/eprllib/agents/holon_config.py` & `eprllib-1.0.9/src/eprllib/agents/holon_config.py`

 * *Files identical despite different names*

### Comparing `eprllib-1.0.8/src/eprllib/agents/user.py` & `eprllib-1.0.9/src/eprllib/agents/user.py`

 * *Files identical despite different names*

### Comparing `eprllib-1.0.8/src/eprllib/env/multiagent/marl_ep_gym_env.py` & `eprllib-1.0.9/src/eprllib/env/multiagent/marl_ep_gym_env.py`

 * *Files identical despite different names*

### Comparing `eprllib-1.0.8/src/eprllib/env/multiagent/marl_ep_runner.py` & `eprllib-1.0.9/src/eprllib/env/multiagent/marl_ep_runner.py`

 * *Files identical despite different names*

### Comparing `eprllib-1.0.8/src/eprllib/env/simpleagent/VENT_ep_gym_env.py` & `eprllib-1.0.9/src/eprllib/env/simpleagent/VENT_ep_gym_env.py`

 * *Files identical despite different names*

### Comparing `eprllib-1.0.8/src/eprllib/env/simpleagent/VENT_ep_runner.py` & `eprllib-1.0.9/src/eprllib/env/simpleagent/VENT_ep_runner.py`

 * *Files identical despite different names*

### Comparing `eprllib-1.0.8/src/eprllib/postprocess/VENT_init_conventional.py` & `eprllib-1.0.9/src/eprllib/postprocess/VENT_init_conventional.py`

 * *Files identical despite different names*

### Comparing `eprllib-1.0.8/src/eprllib/postprocess/VENT_init_conventional_test.py` & `eprllib-1.0.9/src/eprllib/postprocess/VENT_init_conventional_test.py`

 * *Files identical despite different names*

### Comparing `eprllib-1.0.8/src/eprllib/postprocess/VENT_init_evaluation.py` & `eprllib-1.0.9/src/eprllib/postprocess/VENT_init_evaluation.py`

 * *Files identical despite different names*

### Comparing `eprllib-1.0.8/src/eprllib/postprocess/marl_init_conventional.py` & `eprllib-1.0.9/src/eprllib/postprocess/marl_init_conventional.py`

 * *Files identical despite different names*

### Comparing `eprllib-1.0.8/src/eprllib/postprocess/marl_init_evaluation.py` & `eprllib-1.0.9/src/eprllib/postprocess/marl_init_evaluation.py`

 * *Files identical despite different names*

### Comparing `eprllib-1.0.8/src/eprllib/postprocess/marl_init_noventilation.py` & `eprllib-1.0.9/src/eprllib/postprocess/marl_init_noventilation.py`

 * *Files identical despite different names*

### Comparing `eprllib-1.0.8/src/eprllib/postprocess/marl_results_evaluation.ipynb` & `eprllib-1.0.9/src/eprllib/postprocess/marl_results_evaluation.ipynb`

 * *Files identical despite different names*

### Comparing `eprllib-1.0.8/src/eprllib/postprocess/neural_networ_analysis.ipynb` & `eprllib-1.0.9/src/eprllib/postprocess/neural_networ_analysis.ipynb`

 * *Files identical despite different names*

### Comparing `eprllib-1.0.8/src/eprllib/postprocess/results_evaluation.ipynb` & `eprllib-1.0.9/src/eprllib/postprocess/results_evaluation.ipynb`

 * *Files identical despite different names*

### Comparing `eprllib-1.0.8/src/eprllib/postprocess/results_evaluation_test.ipynb` & `eprllib-1.0.9/src/eprllib/postprocess/results_evaluation_test.ipynb`

 * *Files identical despite different names*

### Comparing `eprllib-1.0.8/src/eprllib/postprocess/test_results_evaluation.ipynb` & `eprllib-1.0.9/src/eprllib/postprocess/test_results_evaluation.ipynb`

 * *Files identical despite different names*

### Comparing `eprllib-1.0.8/src/eprllib/preprocess/conventional_experience.py` & `eprllib-1.0.9/src/eprllib/preprocess/conventional_experience.py`

 * *Files identical despite different names*

### Comparing `eprllib-1.0.8/src/eprllib/tools/action_transformers.py` & `eprllib-1.0.9/src/eprllib/tools/action_transformers.py`

 * *Files identical despite different names*

### Comparing `eprllib-1.0.8/src/eprllib/tools/devices_space_action.py` & `eprllib-1.0.9/src/eprllib/tools/devices_space_action.py`

 * *Files identical despite different names*

### Comparing `eprllib-1.0.8/src/eprllib/tools/ep_episode_config.py` & `eprllib-1.0.9/src/eprllib/tools/ep_episode_config.py`

 * *Files identical despite different names*

### Comparing `eprllib-1.0.8/src/eprllib/tools/rewards.py` & `eprllib-1.0.9/src/eprllib/tools/rewards.py`

 * *Files identical despite different names*

### Comparing `eprllib-1.0.8/src/eprllib/tools/weather_utils.py` & `eprllib-1.0.9/src/eprllib/tools/weather_utils.py`

 * *Files identical despite different names*

### Comparing `eprllib-1.0.8/PKG-INFO` & `eprllib-1.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eprllib
-Version: 1.0.8
+Version: 1.0.9
 Summary: Building control trought DRL.
 Author: Germán Rodolfo Henderson
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

