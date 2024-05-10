# Comparing `tmp/loopquest-0.2.2.tar.gz` & `tmp/loopquest-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "loopquest-0.2.2.tar", last modified: Fri May  3 16:54:35 2024, max compression
+gzip compressed data, was "loopquest-0.2.3.tar", last modified: Fri May 10 18:24:36 2024, max compression
```

## Comparing `loopquest-0.2.2.tar` & `loopquest-0.2.3.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxr-x   0 jinyu     (1000) jinyu     (1000)        0 2024-05-03 16:54:35.259745 loopquest-0.2.2/
--rw-rw-r--   0 jinyu     (1000) jinyu     (1000)    11357 2024-04-19 04:42:45.000000 loopquest-0.2.2/LICENSE
--rw-r--r--   0 jinyu     (1000) jinyu     (1000)     6605 2024-05-03 16:54:35.259745 loopquest-0.2.2/PKG-INFO
--rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     5418 2024-04-29 17:12:15.000000 loopquest-0.2.2/README.md
-drwxrwxr-x   0 jinyu     (1000) jinyu     (1000)        0 2024-05-03 16:54:35.255745 loopquest-0.2.2/loopquest/
--rw-rw-r--   0 jinyu     (1000) jinyu     (1000)       86 2024-04-24 04:38:12.000000 loopquest-0.2.2/loopquest/__init__.py
--rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     1439 2024-04-24 05:33:47.000000 loopquest-0.2.2/loopquest/api.py
--rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     9416 2024-05-03 05:47:41.000000 loopquest-0.2.2/loopquest/crud.py
--rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     1933 2024-04-19 04:43:26.000000 loopquest-0.2.2/loopquest/datasets.py
-drwxrwxr-x   0 jinyu     (1000) jinyu     (1000)        0 2024-05-03 16:54:35.255745 loopquest-0.2.2/loopquest/env/
--rw-rw-r--   0 jinyu     (1000) jinyu     (1000)        0 2024-05-01 05:17:29.000000 loopquest-0.2.2/loopquest/env/__init__.py
--rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     4217 2024-04-29 05:10:05.000000 loopquest-0.2.2/loopquest/env/api.py
--rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     6340 2024-05-03 16:52:23.000000 loopquest-0.2.2/loopquest/env/gym_wrappers.py
--rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     9238 2024-04-19 04:43:26.000000 loopquest-0.2.2/loopquest/env/space_utils.py
--rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     5145 2024-04-29 04:54:43.000000 loopquest-0.2.2/loopquest/eval.py
-drwxrwxr-x   0 jinyu     (1000) jinyu     (1000)        0 2024-05-03 16:54:35.255745 loopquest-0.2.2/loopquest/policy/
--rw-rw-r--   0 jinyu     (1000) jinyu     (1000)        0 2024-04-19 04:43:26.000000 loopquest-0.2.2/loopquest/policy/__init__.py
--rw-rw-r--   0 jinyu     (1000) jinyu     (1000)      173 2024-04-19 04:43:26.000000 loopquest-0.2.2/loopquest/policy/base.py
--rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     1383 2024-04-19 04:43:26.000000 loopquest-0.2.2/loopquest/policy/sb3_policy.py
--rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     2001 2024-05-03 04:41:02.000000 loopquest-0.2.2/loopquest/private_api.py
--rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     5685 2024-04-28 05:00:52.000000 loopquest-0.2.2/loopquest/schema.py
--rw-rw-r--   0 jinyu     (1000) jinyu     (1000)      168 2024-04-19 04:43:26.000000 loopquest-0.2.2/loopquest/typing.py
--rw-rw-r--   0 jinyu     (1000) jinyu     (1000)      376 2024-04-19 04:42:45.000000 loopquest-0.2.2/loopquest/ui.py
--rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     4740 2024-05-03 05:20:31.000000 loopquest-0.2.2/loopquest/utils.py
-drwxrwxr-x   0 jinyu     (1000) jinyu     (1000)        0 2024-05-03 16:54:35.255745 loopquest-0.2.2/loopquest.egg-info/
--rw-r--r--   0 jinyu     (1000) jinyu     (1000)     6605 2024-05-03 16:54:35.000000 loopquest-0.2.2/loopquest.egg-info/PKG-INFO
--rw-rw-r--   0 jinyu     (1000) jinyu     (1000)      578 2024-05-03 16:54:35.000000 loopquest-0.2.2/loopquest.egg-info/SOURCES.txt
--rw-rw-r--   0 jinyu     (1000) jinyu     (1000)        1 2024-05-03 16:54:35.000000 loopquest-0.2.2/loopquest.egg-info/dependency_links.txt
--rw-rw-r--   0 jinyu     (1000) jinyu     (1000)      302 2024-05-03 16:54:35.000000 loopquest-0.2.2/loopquest.egg-info/requires.txt
--rw-rw-r--   0 jinyu     (1000) jinyu     (1000)       10 2024-05-03 16:54:35.000000 loopquest-0.2.2/loopquest.egg-info/top_level.txt
--rw-rw-r--   0 jinyu     (1000) jinyu     (1000)       38 2024-05-03 16:54:35.259745 loopquest-0.2.2/setup.cfg
--rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     1144 2024-05-03 16:53:36.000000 loopquest-0.2.2/setup.py
+drwxrwxr-x   0 jinyu     (1000) jinyu     (1000)        0 2024-05-10 18:24:36.929194 loopquest-0.2.3/
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)    11357 2024-04-19 04:42:45.000000 loopquest-0.2.3/LICENSE
+-rw-r--r--   0 jinyu     (1000) jinyu     (1000)     6605 2024-05-10 18:24:36.929194 loopquest-0.2.3/PKG-INFO
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     5418 2024-04-29 17:12:15.000000 loopquest-0.2.3/README.md
+drwxrwxr-x   0 jinyu     (1000) jinyu     (1000)        0 2024-05-10 18:24:36.925194 loopquest-0.2.3/loopquest/
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)       86 2024-04-24 04:38:12.000000 loopquest-0.2.3/loopquest/__init__.py
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     1517 2024-05-08 05:44:07.000000 loopquest-0.2.3/loopquest/api.py
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     9495 2024-05-08 05:56:32.000000 loopquest-0.2.3/loopquest/crud.py
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     1933 2024-04-19 04:43:26.000000 loopquest-0.2.3/loopquest/datasets.py
+drwxrwxr-x   0 jinyu     (1000) jinyu     (1000)        0 2024-05-10 18:24:36.925194 loopquest-0.2.3/loopquest/env/
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)        0 2024-05-01 05:17:29.000000 loopquest-0.2.3/loopquest/env/__init__.py
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     4768 2024-05-08 06:15:15.000000 loopquest-0.2.3/loopquest/env/api.py
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     6392 2024-05-08 05:46:32.000000 loopquest-0.2.3/loopquest/env/gym_wrappers.py
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     9238 2024-04-19 04:43:26.000000 loopquest-0.2.3/loopquest/env/space_utils.py
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     6293 2024-05-10 17:45:41.000000 loopquest-0.2.3/loopquest/eval.py
+drwxrwxr-x   0 jinyu     (1000) jinyu     (1000)        0 2024-05-10 18:24:36.925194 loopquest-0.2.3/loopquest/policy/
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)        0 2024-04-19 04:43:26.000000 loopquest-0.2.3/loopquest/policy/__init__.py
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)      321 2024-05-08 05:05:33.000000 loopquest-0.2.3/loopquest/policy/base.py
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     1383 2024-04-19 04:43:26.000000 loopquest-0.2.3/loopquest/policy/sb3_policy.py
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     2001 2024-05-03 04:41:02.000000 loopquest-0.2.3/loopquest/private_api.py
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     5717 2024-05-09 02:52:37.000000 loopquest-0.2.3/loopquest/schema.py
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)      168 2024-04-19 04:43:26.000000 loopquest-0.2.3/loopquest/typing.py
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)      376 2024-04-19 04:42:45.000000 loopquest-0.2.3/loopquest/ui.py
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     4740 2024-05-03 05:20:31.000000 loopquest-0.2.3/loopquest/utils.py
+drwxrwxr-x   0 jinyu     (1000) jinyu     (1000)        0 2024-05-10 18:24:36.925194 loopquest-0.2.3/loopquest.egg-info/
+-rw-r--r--   0 jinyu     (1000) jinyu     (1000)     6605 2024-05-10 18:24:36.000000 loopquest-0.2.3/loopquest.egg-info/PKG-INFO
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)      578 2024-05-10 18:24:36.000000 loopquest-0.2.3/loopquest.egg-info/SOURCES.txt
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)        1 2024-05-10 18:24:36.000000 loopquest-0.2.3/loopquest.egg-info/dependency_links.txt
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)      302 2024-05-10 18:24:36.000000 loopquest-0.2.3/loopquest.egg-info/requires.txt
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)       10 2024-05-10 18:24:36.000000 loopquest-0.2.3/loopquest.egg-info/top_level.txt
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)       38 2024-05-10 18:24:36.929194 loopquest-0.2.3/setup.cfg
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     1144 2024-05-10 18:24:15.000000 loopquest-0.2.3/setup.py
```

### Comparing `loopquest-0.2.2/LICENSE` & `loopquest-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `loopquest-0.2.2/PKG-INFO` & `loopquest-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: loopquest
-Version: 0.2.2
+Version: 0.2.3
 Summary: A Production Tool for Embodied AI.
 Home-page: https://github.com/LoopMind-AI/loopquest
 Author: LoopMind
 Author-email: contactus@loopmind.ai
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `loopquest-0.2.2/README.md` & `loopquest-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `loopquest-0.2.2/loopquest/api.py` & `loopquest-0.2.3/loopquest/api.py`

 * *Files 19% similar despite different names*

```diff
@@ -48,9 +48,11 @@
     return CLOUD_FRONTEND_URL
 
 
 def get_backend_url():
     return CLOUD_BACKEND_URL
 
 
-def get_user_id():
-    return get_cloud_user_id(get_backend_url())
+def get_user_id(backend_url=None):
+    if backend_url is None:
+        backend_url = get_backend_url()
+    return get_cloud_user_id(backend_url)
```

### Comparing `loopquest-0.2.2/loopquest/crud.py` & `loopquest-0.2.3/loopquest/crud.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,22 +25,23 @@
 from dotenv import load_dotenv
 import os
 from requests.exceptions import HTTPError
 
 load_dotenv()
 
 
-def make_request(method: str, url: str, **kwargs):
-    if TOKEN_ENV_VAR_NAME not in os.environ:
-        raise Exception(
-            f"Please run loopquest.init() before calling other loopquest functions."
-        )
-    headers = kwargs.get("headers", {})
-    headers["Authorization"] = f"Bearer {os.getenv(TOKEN_ENV_VAR_NAME)}"
-    kwargs["headers"] = headers
+def make_request(method: str, url: str, skip_auth_check=False, **kwargs):
+    if not skip_auth_check:
+        if TOKEN_ENV_VAR_NAME not in os.environ:
+            raise Exception(
+                f"Please run loopquest.init() before calling other loopquest functions."
+            )
+        headers = kwargs.get("headers", {})
+        headers["Authorization"] = f"Bearer {os.getenv(TOKEN_ENV_VAR_NAME)}"
+        kwargs["headers"] = headers
 
     try:
         response = requests.request(method, url, **kwargs)
         response.raise_for_status()
     except HTTPError as e:
         if e.response.status_code == 500:
             raise Exception(
```

### Comparing `loopquest-0.2.2/loopquest/datasets.py` & `loopquest-0.2.3/loopquest/datasets.py`

 * *Files identical despite different names*

### Comparing `loopquest-0.2.2/loopquest/env/api.py` & `loopquest-0.2.3/loopquest/env/api.py`

 * *Files 18% similar despite different names*

```diff
@@ -13,14 +13,16 @@
     project_description: str = None,
     experiment_name: str = None,
     experiment_description: str = "",
     experiment_configs: dict[str, Any] = None,
     episode: int = 0,
     use_thread_pool: bool = True,
     max_workers: int = 10,
+    frontend_url: str = None,
+    backend_url: str = None,
     **kwargs,
 ) -> LoopquestGymWrapper:
     """
     Creates a Loopquest environment.
 
     Args:
         env_id (str): The OpenAI Gym environment id to be used.
@@ -35,86 +37,103 @@
 
     Returns:
         LoopquestGymWrapper: The Loopquest environment wrapped with the LoopquestGymWrapper.
 
     Raises:
         Exception: If the experiment is already added to another project or if adding the experiment to the project fails.
     """
+    if frontend_url is None:
+        frontend_url = get_frontend_url()
+    if backend_url is None:
+        backend_url = get_backend_url()
+
     env = gym.make(env_id, **kwargs)
 
     if project_name is None:
         project_name = generate_project_name()
 
     if experiment_name is None:
         experiment_name = generate_experiment_name()
 
     backend_env_ids, experiment = get_or_create_bundle(
-        get_backend_url(),
+        backend_url,
+        # This will always use the default backend_url
         get_user_id(),
         [env],
         project_name,
         project_description,
         experiment_name,
         experiment_description,
         experiment_configs,
     )
 
     print(
-        f"Check the results of experiment {experiment.name} at: {get_frontend_url()}/project/{experiment.project_id}?exp_id={experiment.id}"
+        f"Check the results of experiment {experiment.name} at: {frontend_url}/project/{experiment.project_id}?exp_id={experiment.id}"
     )
     return LoopquestGymWrapper(
         env,
         backend_env_ids[0],
         experiment.id,
         episode=episode,
         use_thread_pool=use_thread_pool,
         max_workers=max_workers,
+        backend_url=backend_url,
     )
 
 
 def make_vec_env(
     env_ids: str,
     project_name: str = None,
     project_description: str = None,
     experiment_name: str = None,
     experiment_description: str = "",
     experiment_configs: dict[str, Any] = None,
     episode: int = 0,
     use_thread_pool: bool = True,
     max_workers: int = 10,
+    frontend_url: str = None,
+    backend_url: str = None,
     **kwargs,
 ) -> VecEnv:
+    if frontend_url is None:
+        frontend_url = get_frontend_url()
+
+    if backend_url is None:
+        backend_url = get_backend_url()
+
     gym_envs = [gym.make(env_id, **kwargs) for env_id in env_ids]
 
     if project_name is None:
         project_name = generate_project_name()
 
     if experiment_name is None:
         experiment_name = generate_experiment_name()
     backend_env_ids, experiment = get_or_create_bundle(
-        get_backend_url(),
+        backend_url,
+        # This will always use the default backend_url
         get_user_id(),
         gym_envs,
         project_name,
         project_description,
         experiment_name,
         experiment_description,
         experiment_configs,
     )
     print(
-        f"Check the results of experiment {experiment.name} at: {get_frontend_url()}/project/{experiment.project_id}?exp_id={experiment.id}"
+        f"Check the results of experiment {experiment.name} at: {frontend_url}/project/{experiment.project_id}?exp_id={experiment.id}"
     )
 
     env_fun = lambda env, backend_env_id: LoopquestGymWrapper(
         env,
         backend_env_id,
         experiment.id,
         episode=episode,
         use_thread_pool=use_thread_pool,
         max_workers=max_workers,
+        backend_url=backend_url,
     )
     return DummyVecEnv(
         [
             lambda: env_fun(env, backend_env_id)
             for env, backend_env_id in zip(gym_envs, backend_env_ids)
         ]
     )
```

### Comparing `loopquest-0.2.2/loopquest/env/gym_wrappers.py` & `loopquest-0.2.3/loopquest/env/gym_wrappers.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,33 +7,35 @@
     update_experiment,
     upload_rgb_as_image,
     get_image_by_url,
 )
 from ..schema import StepCreate, ExperimentUpdate, ExperimentStatus, EnvironmentUpdate
 from ..utils import safe_jsonize
 from .space_utils import construct_space_val
-from ..api import get_backend_url, get_user_id
+from ..api import get_backend_url
 from concurrent.futures import ThreadPoolExecutor
 
 
 class LoopquestGymWrapper(gymnasium.Wrapper):
     def __init__(
         self,
         env: gymnasium.Env,
         env_id: str,
         exp_id: str,
         episode: int = 0,
         use_thread_pool: bool = True,
         max_workers: int = 10,
+        backend_url: str = None,
     ):
         super().__init__(env)
         self.current_step = 0
         self.episode = episode
-        self.backend_url = get_backend_url()
-        self.user_id = get_user_id()
+        if backend_url is None:
+            backend_url = get_backend_url()
+        self.backend_url = backend_url
         self._env_id = env_id
         self._exp_id = exp_id
         self.use_thread_pool = use_thread_pool
         self.executor = None
         if self.use_thread_pool:
             # TODO: evaluate if message queue is better than thread pool.
             self.executor = ThreadPoolExecutor(max_workers=max_workers)
@@ -135,15 +137,15 @@
         # TODO: add a callback to compute custom metrics.
 
     def _try_update_env_profile_image(self):
         env_info = get_environment(self.backend_url, self.cloud_env_id)
         env_update = EnvironmentUpdate()
         if env_info.profile_image is None:
             step_id = f"{self.exp_id}-{self.cloud_env_id}-0-1"
-            image_url = get_backend_url() + f"/step/{step_id}/image/0"
+            image_url = self.backend_url + f"/step/{step_id}/image/0"
             try:
                 img = get_image_by_url(image_url)
                 env_update.profile_image = image_url
             except Exception as e:
                 print(e)
         update_environment(self.backend_url, self.cloud_env_id, env_update)
```

### Comparing `loopquest-0.2.2/loopquest/env/space_utils.py` & `loopquest-0.2.3/loopquest/env/space_utils.py`

 * *Files identical despite different names*

### Comparing `loopquest-0.2.2/loopquest/eval.py` & `loopquest-0.2.3/loopquest/eval.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from .policy.base import BasePolicy
 from typing import Any
 import gymnasium as gym
 from .utils import generate_experiment_name, generate_project_name
 from .api import get_user_id, get_backend_url, get_frontend_url
-from .crud import get_or_create_bundle
+from .crud import get_or_create_bundle, update_experiment
+from .schema import ExperimentStatus, ExperimentUpdate
 from .env.gym_wrappers import LoopquestGymWrapper
 from .policy.sb3_policy import SB3Policy
 from tqdm import tqdm
 from huggingface_sb3 import load_from_hub
 
 
 def evaluate_local_policy(
@@ -22,15 +23,26 @@
     experiment_configs: dict[str, Any] = None,
     policy_filename: str = None,
     policy_repo_id: str = None,
     algorithm_name: str = None,
     use_thread_pool: bool = True,
     max_workers: int = 10,
     disable_progress_bar: bool = False,
+    frontend_url: str = None,
+    backend_url: str = None,
+    user_id: str = None,
 ):
+    if backend_url is None:
+        backend_url = get_backend_url()
+
+    if frontend_url is None:
+        frontend_url = get_frontend_url()
+
+    if user_id is None:
+        user_id = get_user_id()
 
     gym_envs = [gym.make(env_id) for env_id in env_ids]
     if all(["rgb_array" in env.metadata.get("render_modes", []) for env in gym_envs]):
         render_mode = "rgb_array"
     elif all(
         ["rgb_array_list" in env.metadata.get("render_modes", []) for env in gym_envs]
     ):
@@ -44,71 +56,84 @@
     if project_name is None:
         project_name = generate_project_name()
 
     if experiment_name is None:
         experiment_name = generate_experiment_name()
 
     backend_env_ids, experiment = get_or_create_bundle(
-        get_backend_url(),
-        get_user_id(),
+        backend_url,
+        user_id,
         gym_envs,
         project_name,
         project_description,
         experiment_name,
         experiment_description,
         experiment_configs,
         policy_filename=policy_filename,
         policy_repo_id=policy_repo_id,
         algorithm_name=algorithm_name,
         num_episodes=num_episodes,
         num_steps=num_steps_per_episode,
     )
 
-    frontend_url = get_frontend_url()
     print(
         f"Check the results of experiment {experiment.name} at: {frontend_url}/project/{experiment.project_id}?exp_id={experiment.id}"
     )
 
     # TODO: the dummy for loop can be replaced by parallelism.
-    for eps in tqdm(range(num_episodes), desc="Episodes", disable=disable_progress_bar):
-        # NOTE: we did not use vec env because vec env requires all the envs run
-        # to the same time steps, but envs terminate at different time steps.
-        for env_id, backend_env_id in tqdm(
-            zip(env_ids, backend_env_ids),
-            total=len(gym_envs),
-            desc="Environments",
-            leave=False,
-            disable=disable_progress_bar,
+    try:
+        for eps in tqdm(
+            range(num_episodes), desc="Episodes", disable=disable_progress_bar
         ):
-            env = LoopquestGymWrapper(
-                # NOTE: Making env every time to avoid the env state being
-                # changed and renderer does not work as expected etc., but this
-                # might hurt performance.
-                gym.make(env_id, render_mode=render_mode),
-                backend_env_id,
-                experiment.id,
-                episode=eps,
-                use_thread_pool=use_thread_pool,
-                max_workers=max_workers,
-            )
-
-            obs, info = env.reset()
-            for _ in tqdm(
-                range(num_steps_per_episode),
-                desc="Steps",
+            # NOTE: we did not use vec env because vec env requires all the envs run
+            # to the same time steps, but envs terminate at different time steps.
+            for env_id, backend_env_id in tqdm(
+                zip(env_ids, backend_env_ids),
+                total=len(gym_envs),
+                desc="Environments",
                 leave=False,
                 disable=disable_progress_bar,
             ):
-                action = policy.compute_action(obs)
-                obs, reward, terminated, truncated, info = env.step(action)
-                if render_mode in ["rgb_array", "rgb_array_list"]:
-                    env.render()
-                if terminated or truncated:
-                    break
-            env.close()
+                env = LoopquestGymWrapper(
+                    # NOTE: Making env every time to avoid the env state being
+                    # changed and renderer does not work as expected etc., but this
+                    # might hurt performance.
+                    gym.make(env_id, render_mode=render_mode),
+                    backend_env_id,
+                    experiment.id,
+                    episode=eps,
+                    use_thread_pool=use_thread_pool,
+                    max_workers=max_workers,
+                    backend_url=backend_url,
+                )
+                policy.set_action_space(env.action_space)
+                obs, info = env.reset()
+                for _ in tqdm(
+                    range(num_steps_per_episode),
+                    desc="Steps",
+                    leave=False,
+                    disable=disable_progress_bar,
+                ):
+                    action = policy.compute_action(obs)
+                    obs, reward, terminated, truncated, info = env.step(action)
+                    if render_mode in ["rgb_array", "rgb_array_list"]:
+                        env.render()
+                    if terminated or truncated:
+                        break
+                env.close()
+    except Exception as e:
+        update_experiment(
+            backend_url,
+            experiment.id,
+            ExperimentUpdate(
+                status=ExperimentStatus.FAILED,
+                error_message=str(e),
+            ),
+        )
+    return experiment.id, experiment.project_id
 
 
 # Only supports stable baseline3 policies in huggingface for now.
 def evaluate_remote_policy(
     huggingface_repo_id: str,
     huggingface_filename: str,
     algorithm_name: str,
@@ -118,29 +143,37 @@
     project_name: str = None,
     project_description: str = None,
     experiment_name: str = None,
     experiment_description: str = "",
     experiment_configs: dict[str, Any] = None,
     use_thread_pool: bool = True,
     max_workers: int = 10,
+    disable_progress_bar: bool = False,
+    frontend_url: str = None,
+    backend_url: str = None,
+    user_id: str = None,
 ):
     checkpoint = load_from_hub(
         repo_id=huggingface_repo_id,
         filename=huggingface_filename,
     )
     policy = SB3Policy.load(checkpoint, algorithm_name)
-    evaluate_local_policy(
+    return evaluate_local_policy(
         policy,
         env_ids,
         num_episodes=num_episodes,
         num_steps_per_episode=num_steps_per_episode,
         project_name=project_name,
         project_description=project_description,
         experiment_name=experiment_name,
         experiment_description=experiment_description,
         experiment_configs=experiment_configs,
         use_thread_pool=use_thread_pool,
         max_workers=max_workers,
         policy_filename=huggingface_filename,
         policy_repo_id=huggingface_repo_id,
         algorithm_name=algorithm_name,
+        disable_progress_bar=disable_progress_bar,
+        frontend_url=frontend_url,
+        backend_url=backend_url,
+        user_id=user_id,
     )
```

### Comparing `loopquest-0.2.2/loopquest/policy/sb3_policy.py` & `loopquest-0.2.3/loopquest/policy/sb3_policy.py`

 * *Files identical despite different names*

### Comparing `loopquest-0.2.2/loopquest/private_api.py` & `loopquest-0.2.3/loopquest/private_api.py`

 * *Files identical despite different names*

### Comparing `loopquest-0.2.2/loopquest/schema.py` & `loopquest-0.2.3/loopquest/schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -167,17 +167,18 @@
     environment_id: Optional[str] = None
     episode: Optional[int] = None
     # In simulation, all the observations and actions are aligned in time.
     step: Optional[int] = None
 
 
 class EvalRequest(BaseModel):
-    huggingface_repo_id: str
-    huggingface_filename: str
-    algorithm_name: str
+    user_id: str
+    huggingface_repo_id: str = ""
+    huggingface_filename: str = ""
+    algorithm_name: str = ""
     env_ids: list[str]
     num_episodes: int = 10
     num_steps_per_episode: int = 1000
     project_name: str = None
     project_description: str = None
     experiment_name: str = None
     experiment_description: str = ""
```

### Comparing `loopquest-0.2.2/loopquest/utils.py` & `loopquest-0.2.3/loopquest/utils.py`

 * *Files identical despite different names*

### Comparing `loopquest-0.2.2/loopquest.egg-info/PKG-INFO` & `loopquest-0.2.3/loopquest.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: loopquest
-Version: 0.2.2
+Version: 0.2.3
 Summary: A Production Tool for Embodied AI.
 Home-page: https://github.com/LoopMind-AI/loopquest
 Author: LoopMind
 Author-email: contactus@loopmind.ai
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `loopquest-0.2.2/loopquest.egg-info/SOURCES.txt` & `loopquest-0.2.3/loopquest.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `loopquest-0.2.2/setup.py` & `loopquest-0.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="loopquest",
-    version="0.2.2",
+    version="0.2.3",
     description="A Production Tool for Embodied AI.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="LoopMind",
     author_email="contactus@loopmind.ai",
     url="https://github.com/LoopMind-AI/loopquest",
     packages=find_packages(),
```

