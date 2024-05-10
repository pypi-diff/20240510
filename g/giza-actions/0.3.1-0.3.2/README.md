# Comparing `tmp/giza_actions-0.3.1.tar.gz` & `tmp/giza_actions-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "giza_actions-0.3.1.tar", max compression
+gzip compressed data, was "giza_actions-0.3.2.tar", max compression
```

## Comparing `giza_actions-0.3.1.tar` & `giza_actions-0.3.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1074 2024-04-22 16:09:43.755393 giza_actions-0.3.1/LICENSE
--rw-r--r--   0        0        0     6353 2024-04-22 16:09:43.755393 giza_actions-0.3.1/README.md
--rw-r--r--   0        0        0      243 2024-04-22 16:09:43.767393 giza_actions-0.3.1/giza_actions/__init__.py
--rw-r--r--   0        0        0     5906 2024-04-22 16:09:43.767393 giza_actions-0.3.1/giza_actions/action.py
--rw-r--r--   0        0        0    17175 2024-04-22 16:09:43.767393 giza_actions-0.3.1/giza_actions/agent.py
--rw-r--r--   0        0        0      601 2024-04-22 16:09:43.767393 giza_actions-0.3.1/giza_actions/deployments.py
--rw-r--r--   0        0        0      225 2024-04-22 16:09:43.767393 giza_actions-0.3.1/giza_actions/logger.py
--rw-r--r--   0        0        0     3051 2024-04-22 16:09:43.767393 giza_actions-0.3.1/giza_actions/logging.yaml
--rw-r--r--   0        0        0    15596 2024-04-22 16:09:43.767393 giza_actions-0.3.1/giza_actions/model.py
--rw-r--r--   0        0        0      519 2024-04-22 16:09:43.767393 giza_actions-0.3.1/giza_actions/task.py
--rw-r--r--   0        0        0     1907 2024-04-22 16:09:43.767393 giza_actions-0.3.1/giza_actions/utils.py
--rw-r--r--   0        0        0     1282 2024-04-22 16:09:43.771393 giza_actions-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     7432 1970-01-01 00:00:00.000000 giza_actions-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1074 2024-05-10 14:58:21.741931 giza_actions-0.3.2/LICENSE
+-rw-r--r--   0        0        0     6353 2024-05-10 14:58:21.741931 giza_actions-0.3.2/README.md
+-rw-r--r--   0        0        0      243 2024-05-10 14:58:21.753931 giza_actions-0.3.2/giza_actions/__init__.py
+-rw-r--r--   0        0        0     5993 2024-05-10 14:58:21.753931 giza_actions-0.3.2/giza_actions/action.py
+-rw-r--r--   0        0        0    17767 2024-05-10 14:58:21.753931 giza_actions-0.3.2/giza_actions/agent.py
+-rw-r--r--   0        0        0      631 2024-05-10 14:58:21.753931 giza_actions-0.3.2/giza_actions/deployments.py
+-rw-r--r--   0        0        0      252 2024-05-10 14:58:21.753931 giza_actions-0.3.2/giza_actions/logger.py
+-rw-r--r--   0        0        0     3051 2024-05-10 14:58:21.753931 giza_actions-0.3.2/giza_actions/logging.yaml
+-rw-r--r--   0        0        0    18134 2024-05-10 14:58:21.753931 giza_actions-0.3.2/giza_actions/model.py
+-rw-r--r--   0        0        0      576 2024-05-10 14:58:21.753931 giza_actions-0.3.2/giza_actions/task.py
+-rw-r--r--   0        0        0     1966 2024-05-10 14:58:21.753931 giza_actions-0.3.2/giza_actions/utils.py
+-rw-r--r--   0        0        0     1303 2024-05-10 14:58:21.757932 giza_actions-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     7474 1970-01-01 00:00:00.000000 giza_actions-0.3.2/PKG-INFO
```

### Comparing `giza_actions-0.3.1/LICENSE` & `giza_actions-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `giza_actions-0.3.1/README.md` & `giza_actions-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `giza_actions-0.3.1/giza_actions/action.py` & `giza_actions-0.3.2/giza_actions/action.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 from functools import partial, wraps
 from pathlib import Path
-from typing import Optional
+from typing import Any, Callable, Optional
 
 from giza_actions.utils import get_workspace_uri  # noqa: E402
 
 os.environ["PREFECT_API_URL"] = f"{get_workspace_uri()}/api"
 os.environ["PREFECT_UI_URL"] = get_workspace_uri()
 
 from prefect import Flow  # noqa: E402
@@ -47,33 +47,33 @@
             entrypoint (Flow): The Prefect flow that represents the action's entrypoint.
             name (str): The name of the action.
         """
         self.name = name
         self._flow = entrypoint
         self._set_settings()
 
-    def _set_settings(self):
+    def _set_settings(self) -> None:
         """
         Updates the current profile with the workspace API URL and the path to the logging configuration.
         """
         update_current_profile(settings={PREFECT_API_URL: f"{get_workspace_uri()}/api"})
         update_current_profile(
             settings={PREFECT_LOGGING_SETTINGS_PATH: f"{__module_path__}/logging.yaml"}
         )
 
-    def _update_api_url(self, api_url: str):
+    def _update_api_url(self, api_url: str) -> None:
         """
         Updates the API URL in the current profile.
 
         Args:
             api_url (str): The new API URL to set in the profile.
         """
         update_current_profile(settings={PREFECT_API_URL: api_url})
 
-    def get_flow(self):
+    def get_flow(self) -> Flow:
         """
         Returns the Prefect flow associated with the action.
 
         Returns:
             Flow: The Prefect flow of the action.
         """
         return self._flow
@@ -82,15 +82,15 @@
     async def serve(
         self,
         name: str,
         cron: Optional[str] = None,
         interval: Optional[str] = None,
         parameters: Optional[dict] = None,
         print_starting_message: bool = True,
-    ):
+    ) -> None:
         """
         Serves the action, making it ready to poll for scheduled runs.
 
         Args:
             name (str): The name to assign to the runner. If a file path is provided, it uses the file name without the extension.
             print_starting_message (bool, optional): Whether to print a starting message. Defaults to True.
             interval: An interval on which to schedule runs. Accepts either a number
@@ -138,30 +138,30 @@
                 )
 
             console = Console()
             console.print(Panel(help_message))
         await runner.start(webserver=False)
 
 
-def action(func=None, *task_init_args, **task_init_kwargs):
+def action(func: Callable, *task_init_args: Any, **task_init_kwargs: Any) -> Flow:
     """
     Decorator to convert a function into a Prefect flow.
 
     Args:
         func (Callable, optional): The function to convert into a flow. If None, returns a partial function.
         **task_init_kwargs: Arbitrary keyword arguments passed to the flow initialization.
 
     Returns:
         Flow: The Prefect flow created from the function.
     """
     if func is None:
         return partial(action, *task_init_args, **task_init_kwargs)
 
     @wraps(func)
-    def safe_func(*args, **kwargs):
+    def safe_func(*args: Any, **kwargs: Any) -> Any:
         """
         A wrapper function that calls the original function with its arguments.
 
         Args:
             **kwargs: Arbitrary keyword arguments passed to the original function.
 
         Returns:
```

### Comparing `giza_actions-0.3.1/giza_actions/agent.py` & `giza_actions-0.3.2/giza_actions/agent.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import json
 import logging
 import os
 import time
 from contextlib import contextmanager
 from pathlib import Path
-from typing import Any, Callable, Dict, Optional, Tuple, Union
+from typing import Any, Callable, Dict, Optional, Self, Tuple, Union
 
 from ape import Contract, accounts, networks
 from ape.contracts import ContractInstance
 from ape.exceptions import NetworkError
 from ape_accounts.accounts import InvalidPasswordError
 from giza import API_HOST
 from giza.client import AgentsClient, EndpointsClient, JobsClient, ProofsClient
@@ -30,19 +30,19 @@
     """
 
     # TODO: (GIZ 502) Find a way to abstract away the chain_id to just a string with the chain name
     def __init__(
         self,
         id: int,
         version_id: int,
-        contracts: Optional[Dict[str, str]] = None,
+        contracts: Dict[str, str],
         chain: Optional[str] = None,
         account: Optional[str] = None,
-        **kwargs,
-    ):
+        **kwargs: Any,
+    ) -> None:
         """
         Args:
             model_id (int): The ID of the model.
             version_id (int): The version of the model.
             contracts (Dict[str, str]): The contracts to handle, must be a dictionary with the contract name as the key and the contract address as the value.
             chain_id (int): The ID of the blockchain network.
             **kwargs: Additional keyword arguments.
@@ -83,16 +83,16 @@
     @classmethod
     def from_id(
         cls,
         id: int,
         contracts: Optional[Dict[str, Any]] = None,
         chain: Optional[str] = None,
         account: Optional[str] = None,
-        **kwargs,
-    ):
+        **kwargs: Any,
+    ) -> "GizaAgent":
         """
         Create an agent from an ID.
         """
 
         client: AgentsClient = kwargs.pop("client", AgentsClient(API_HOST))
         try:
             agent: Agent = client.get(id)
@@ -107,15 +107,15 @@
             version_id=agent.parameters["version_id"],
             contracts=contracts if contracts else agent.parameters["contracts"],
             chain=chain if chain else agent.parameters["chain"],
             account=account if account else agent.parameters["account"],
             **kwargs,
         )
 
-    def _check_or_create_account(self):
+    def _check_or_create_account(self) -> None:
         """
         Check if the account exists in the execution environment, if not create it from the agent.
         """
         try:
             accounts.load(self.account)
         except Exception:
             logger.info(
@@ -151,20 +151,20 @@
                     f"Agent with model ID {self.model_id} and version ID {self.version_id} not found"
                 )
             return agents.root[0]
         except HTTPError as e:
             logger.error(f"Failed to get agent: {e}")
             raise ValueError(f"Failed to get agent with id {self.model_id}: {e}")
 
-    def _update_agent(self):
+    def _update_agent(self) -> None:
         """
         Update the agent.
         """
         try:
-            parameters = {}
+            parameters: Dict[Any, Any] = {}
             if (
                 "chain" not in self._agent.parameters
                 or self._agent.parameters["chain"] != self.chain
             ):
                 self._agent.parameters["chain"] = self.chain
                 parameters["chain"] = self.chain
                 logger.info(f"Updating agent with chain {self.chain}")
@@ -176,15 +176,15 @@
                 self._agent.parameters["account"] = self.account
                 parameters["account"] = self.account
                 path = (
                     Path.home()
                     .joinpath(".ape/accounts")
                     .joinpath(f"{self.account}.json")
                 )
-                account_data = read_json(path)
+                account_data = read_json(str(path))
                 parameters["account_data"] = account_data
                 logger.info(f"Updating agent with account {self.account}")
             if (
                 "contracts" not in self._agent.parameters
                 or self._agent.parameters["contracts"]
                 != self.contract_handler._contracts
             ):
@@ -194,40 +194,45 @@
             agent = AgentUpdate(parameters=parameters)
             self._agents_client.patch(self._agent.id, agent)
             logger.info("Agent updated!")
         except HTTPError as e:
             logger.error(f"Failed to update agent: {e}")
             raise ValueError(f"Failed to update agent with id {self.model_id}: {e}")
 
-    def _check_passphrase_in_env(self):
+    def _check_passphrase_in_env(self) -> None:
         """
         Check if the passphrase is in the environment variables.
         """
+        if self.account is None:
+            raise ValueError("Account is not specified.")
+
         if f"{self.account.upper()}_PASSPHRASE" not in os.environ:
             logger.error(
                 f"Passphrase for account {self.account} not found in environment variables. Passphrase must be stored in an environment variable named {self.account.upper()}_PASSPHRASE."
             )
             raise ValueError(
                 f"Passphrase for account {self.account} not found in environment variables"
             )
 
     @contextmanager
-    def execute(self):
+    def execute(self) -> Any:
         """
         Execute the agent in the given ecosystem. Return the contract instace so the user can execute it.
 
         Args:
             ecosystem: The ecosystem to execute the agent in.
         """
         logger.debug("Provider configured")
         self._update_agent()
         with self._provider:
             self._account = accounts.load(self.account)
             logger.debug("Account loaded")
             try:
+                if self.account is None:
+                    raise ValueError("Account is not specified.")
                 self._account.set_autosign(
                     True, passphrase=os.getenv(f"{self.account.upper()}_PASSPHRASE")
                 )
             except InvalidPasswordError as e:
                 logger.error(
                     f"Invalid passphrase for account {self.account}. Could not decrypt account."
                 )
@@ -239,20 +244,20 @@
                 yield self.contract_handler.handle()
 
     def predict(
         self,
         input_file: Optional[str] = None,
         input_feed: Optional[Dict] = None,
         verifiable: bool = False,
-        fp_impl="FP16x16",
+        fp_impl: str = "FP16x16",
         custom_output_dtype: Optional[str] = None,
         job_size: str = "M",
         dry_run: bool = False,
-        **result_kwargs,
-    ) -> Union["AgentResult", Tuple[Any, str]]:
+        **result_kwargs: Any,
+    ) -> Optional[Union[Tuple[Any, Any], "AgentResult"]]:
         """
         Runs a round of inference on the model and saves the result.
 
         Args:
             input_file: The input file to use for inference
             input_feed: The input feed to use for inference
             job_size: The size of the job to run
@@ -271,24 +276,29 @@
 
         if not verifiable:
             logger.warning(
                 "Inference is not verifiable. No request ID was returned. No proof will be generated."
             )
             return result
 
-        pred, request_id = result
-        return AgentResult(
-            input=input_feed,
-            request_id=request_id,
-            result=pred,
-            endpoint_id=self.endpoint_id,
-            agent=self,
-            dry_run=dry_run,
-            **result_kwargs,
-        )
+        if result is None:
+            raise ValueError("The prediction result is None!")
+        if isinstance(result, tuple):
+            pred, request_id = result
+            return AgentResult(
+                input=input_feed,
+                request_id=request_id,
+                result=pred,
+                endpoint_id=self.endpoint_id,
+                agent=self,
+                dry_run=dry_run,
+                **result_kwargs,
+            )
+        else:
+            raise ValueError("We are expecting result to be a tuple!")
 
 
 class AgentResult:
     """
     A class to represent the result of an agent's inference.
     """
 
@@ -297,15 +307,15 @@
         input: Any,
         request_id: str,
         result: Any,
         agent: GizaAgent,
         endpoint_client: EndpointsClient = EndpointsClient(API_HOST),
         jobs_client: JobsClient = JobsClient(API_HOST),
         proofs_client: ProofsClient = ProofsClient(API_HOST),
-        **kwargs,
+        **kwargs: Any,
     ):
         """
         Args:
             input (list): The input to the agent.
             request_id (str): The request ID of the proof.
             value (int): The value of the inference.
         """
@@ -340,38 +350,38 @@
         jobs: JobList = client.list_jobs(self._endpoint_id)
         for job in jobs.root:
             if job.request_id == self.request_id:
                 return job
         raise ValueError(f"Proof job for request ID {self.request_id} not found")
 
     @property
-    def value(self):
+    def value(self) -> Any:
         """
         Get the value of the inference.
         """
         if self.verified:
             return self.__value
         self._verify()
         return self.__value
 
-    def _verify(self):
+    def _verify(self) -> None:
         """
         Verify the proof. Check for the proof job, if its done start the verify job, then wait for verification.
         """
         if self._dry_run:
             logger.warning("Dry run enabled. Skipping verification.")
             self.verified = True
             return
 
         self._wait_for_proof(self._jobs_client, self._timeout, self._poll_interval)
         self.verified = self._verify_proof(self._endpoint_client)
 
     def _wait_for_proof(
         self, client: JobsClient, timeout: int = 600, poll_interval: int = 10
-    ):
+    ) -> None:
         """
         Wait for the proof job to finish.
         """
         self._wait_for(self._proof_job, client, timeout, poll_interval, JobKind.PROOF)
         self._proof = self._endpoint_client.get_proof(
             self._endpoint_id, self._proof_job.request_id
         )
@@ -391,15 +401,15 @@
     def _wait_for(
         self,
         job: Job,
         client: JobsClient,
         timeout: int = 600,
         poll_interval: int = 10,
         kind: JobKind = JobKind.VERIFY,
-    ):
+    ) -> None:
         """
         Wait for a job to finish.
 
         Args:
             job (Job): The job to wait for.
             client (JobsClient): The client to use.
             timeout (int): The timeout.
@@ -452,15 +462,15 @@
 
     def _initiate_contract(self, address: str) -> ContractInstance:
         """
         Initiate the contract.
         """
         return Contract(address=address)
 
-    def handle(self):
+    def handle(self) -> Self:
         """
         Handle the contracts.
         """
         try:
             for name, address in self._contracts.items():
                 self._contracts_instances[name] = self._initiate_contract(address)
         except NetworkError as e:
```

### Comparing `giza_actions-0.3.1/giza_actions/deployments.py` & `giza_actions-0.3.2/giza_actions/deployments.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 import logging
 import os  # noqa: E402
+from typing import Any
 
 from giza_actions.utils import get_workspace_uri  # noqa: E402
 
 os.environ["PREFECT_API_URL"] = f"{get_workspace_uri()}/api"
 os.environ["PREFECT_UI_URL"] = get_workspace_uri()
 
 from prefect.deployments import run_deployment  # noqa: E402
 
 logger = logging.getLogger(__name__)
 
 
-def run_action_deployment(name: str, parameters: dict = None):
+def run_action_deployment(name: str, parameters: dict = None) -> Any:
     deployment_run = run_deployment(name=name, parameters=parameters)
     logger.info(
         f"Deployment run name: {deployment_run.name} exited with state: {deployment_run.state_name}"
     )
     return deployment_run
```

### Comparing `giza_actions-0.3.1/giza_actions/logging.yaml` & `giza_actions-0.3.2/giza_actions/logging.yaml`

 * *Files identical despite different names*

### Comparing `giza_actions-0.3.1/giza_actions/model.py` & `giza_actions-0.3.2/giza_actions/model.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,34 @@
 import logging
+import os
+import tempfile
 from pathlib import Path
-from typing import Dict, Optional
+from typing import TYPE_CHECKING, Any, Dict, Optional, Tuple, Union
 
 import numpy as np
 import onnx
 import onnxruntime as ort
 import requests
+from diskcache import Cache
 from giza import API_HOST
 from giza.client import ApiClient, EndpointsClient, ModelsClient, VersionsClient
+from giza.schemas.models import Model
+from giza.schemas.versions import Version
 from giza.utils.enums import Framework, VersionStatus
 from osiris.app import (
     create_tensor_from_array,
     deserialize,
     load_data,
     serialize,
     serializer,
 )
 
+if TYPE_CHECKING:
+    from giza_actions.agent import AgentResult
+
 from giza_actions.utils import get_endpoint_uri
 
 logger = logging.getLogger(__name__)
 
 
 class GizaModel:
     """
@@ -64,33 +72,42 @@
 
         if model_path and id and version:
             raise ValueError(
                 "Only one of model_path or id and version should be provided."
             )
 
         if model_path:
-            self.session = ort.InferenceSession(model_path)
+            if ".onnx" in model_path:
+                self.session = ort.InferenceSession(model_path)
+            # TODO (@alejandromartinezgotor): if ".json" in model_path create session for non-verifiable inference.
         elif id and version:
             self.model_id = id
             self.version_id = version
             self.model_client = ModelsClient(API_HOST)
             self.version_client = VersionsClient(API_HOST)
             self.api_client = ApiClient(API_HOST)
             self.endpoints_client = EndpointsClient(API_HOST)
             self._get_credentials()
             self.model = self._get_model(id)
             self.version = self._get_version(version)
-            self.session = self._set_session()
             self.framework = self.version.framework
             self.uri = self._retrieve_uri()
             self.endpoint_id = self._get_endpoint_id()
-            if output_path:
-                self._download_model(output_path)
+            self._cache = Cache(os.path.join(os.getcwd(), "tmp", "cachedir"))
+            self.session = self._set_session()
+            if output_path is not None:
+                self._output_path = output_path
+            else:
+                self._output_path = os.path.join(
+                    tempfile.gettempdir(),
+                    f"{self.model_id}_{self.version_id}_{self.model.name}",
+                )
+            self._download_model()
 
-    def _get_endpoint_id(self):
+    def _get_endpoint_id(self) -> int:
         """
         Retrieves the endpoint id for the deployed model.
 
         Returns:
             The endpoint id for the deployed model.
         """
         deployments_list = self.endpoints_client.list(
@@ -104,15 +121,15 @@
         if len(deployments_list.root) == 1:
             return deployments_list.root[0].id
         elif len(deployments_list.root) > 1:
             raise ValueError("Multiple versions deployed for the same model")
         else:
             raise ValueError("No active deployments found")
 
-    def _retrieve_uri(self):
+    def _retrieve_uri(self) -> str:
         """
         Retrieves the URI for making prediction requests to a deployed model.
 
         Args:
             version_id (int): The version number of the model.
 
         Returns:
@@ -121,63 +138,66 @@
         # Different URI per framework
         uri = get_endpoint_uri(self.model.id, self.version.version)
         if self.framework == Framework.CAIRO:
             return f"{uri}/cairo_run"
         else:
             return f"{uri}/predict"
 
-    def _get_model(self, model_id: int):
+    def _get_model(self, model_id: int) -> Model:
         """
         Retrieves the model specified by model_id.
 
         Args:
             model_id (int): The unique identifier of the model.
 
         Returns:
             The model.
         """
         return self.model_client.get(model_id)
 
-    def _get_version(self, version_id: int):
+    def _get_version(self, version_id: int) -> Version:
         """
         Retrieves the version of the model specified by model id and version id.
 
         Args:
             version_id (int): The version number of the model.
 
         Returns:
             The version of the model.
         """
         return self.version_client.get(self.model.id, version_id)
 
-    def _set_session(self):
+    def _set_session(self) -> Optional[ort.InferenceSession]:
         """
         Set onnxruntime session for the model specified by model id.
 
         Raises:
             ValueError: If the model version status is not completed.
         """
 
         if self.version.status != VersionStatus.COMPLETED:
             raise ValueError(
                 f"Model version status is not completed {self.version.status}"
             )
 
         try:
-            onnx_model = self.version_client.download_original(
-                self.model.id, self.version.version
-            )
+            self._download_model()
+
+            if self._output_path in self._cache:
+                file_path = Path(self._cache.get(self._output_path))
+                with open(file_path, "rb") as f:
+                    onnx_model = f.read()
 
             return ort.InferenceSession(onnx_model)
 
         except Exception as e:
             logger.info(f"Could not download model: {e}")
             return None
 
-    def _download_model(self, output_path: str):
+    def _download_model(self) -> None:
         """
         Downloads the model specified by model id and version id to the given output_path.
 
         Args:
             output_path (str): The file path where the downloaded model should be saved.
 
         Raises:
@@ -185,57 +205,64 @@
         """
 
         if self.version.status != VersionStatus.COMPLETED:
             raise ValueError(
                 f"Model version status is not completed {self.version.status}"
             )
 
-        onnx_model = self.version_client.download_original(
-            self.model.id, self.version.version
-        )
+        if self._output_path not in self._cache:
+            onnx_model = self.version_client.download_original(
+                self.model.id, self.version.version
+            )
 
-        logger.info("ONNX model is ready, downloading! ✅")
+            logger.info("Model is ready, downloading! ✅")
 
-        if ".onnx" in output_path:
-            save_path = Path(output_path)
-        else:
-            save_path = Path(f"{output_path}/{self.model.name}.onnx")
+            if (".onnx" or ".json") in self._output_path:
+                save_path = Path(self._output_path)
+            else:
+                save_path = Path(f"{self._output_path}.onnx")
 
-        with open(save_path, "wb") as f:
-            f.write(onnx_model)
+            with open(save_path, "wb") as f:
+                f.write(onnx_model)
 
-        logger.info(f"ONNX model saved at: {save_path} ✅")
+            self._cache[self._output_path] = save_path
+
+            logger.info(f"Model saved at: {save_path} ✅")
+        else:
+            logger.info(f"Model already downloaded at: {self._output_path} ✅")
 
-    def _get_credentials(self):
+    def _get_credentials(self) -> None:
         """
         Retrieves and sets the necessary credentials for API access.
         """
         self.api_client.retrieve_token()
         self.api_client.retrieve_api_key()
 
     def predict(
         self,
         input_file: Optional[str] = None,
         input_feed: Optional[Dict] = None,
         verifiable: bool = False,
-        fp_impl="FP16x16",
+        fp_impl: str = "FP16x16",
         custom_output_dtype: Optional[str] = None,
+        model_category="ONNX_ORION",
         job_size: str = "M",
         dry_run: bool = False,
-    ):
+    ) -> Optional[Union[Tuple[Any, Any], "AgentResult"]]:
         """
         Makes a prediction using either a local ONNX session or a remote deployed model, depending on the
         instance configuration.
 
         Args:
             input_file (Optional[str]): The path to the input file for prediction. Defaults to None.
             input_feed (Optional[Dict]): A dictionary containing the input data for prediction. Defaults to None.
             verifiable (bool): A flag indicating whether to use the verifiable computation endpoint. Defaults to False.
             fp_impl (str): The fixed point implementation to use, when computed in verifiable mode. Defaults to "FP16x16".
             custom_output_dtype (Optional[str]): Specify the data type of the result when computed in verifiable mode. Defaults to None.
+            model_category (str): The category of model. "ONNX_ORION" | "XGB" | "LGBM"
 
         Returns:
             A tuple (predictions, request_id) where predictions is the result of the prediction and request_id
             is the identifier of the prediction request if verifiable computation is used, otherwise None.
 
         Raises:
             ValueError: If required parameters are not provided or the session is not initialized.
@@ -244,15 +271,19 @@
             logger.info("Predicting")
             if verifiable:
                 if not self.uri:
                     raise ValueError("Model has not been deployed")
 
                 # Non common arguments should be named parameters
                 payload = self._format_inputs_for_framework(
-                    input_file, input_feed, fp_impl=fp_impl, job_size=job_size
+                    input_file,
+                    input_feed,
+                    fp_impl=fp_impl,
+                    model_category=model_category,
+                    job_size=job_size,
                 )
 
                 if dry_run:
                     payload["dry_run"] = True
 
                 response = requests.post(self.uri, json=payload)
 
@@ -267,38 +298,44 @@
                 body = response.json()
                 serialized_output = body["result"]
                 request_id = body["request_id"]
 
                 if self.framework == Framework.CAIRO:
                     logger.info("Serialized: %s", serialized_output)
 
-                    if custom_output_dtype is None:
-                        output_dtype = self._get_output_dtype()
-                    else:
-                        output_dtype = custom_output_dtype
+                    if model_category == "ONNX_ORION":
+                        if custom_output_dtype is None:
+                            output_dtype = self._get_output_dtype()
+                        else:
+                            output_dtype = custom_output_dtype
+                    elif model_category in ["XGB", "LGBM"]:
+                        output_dtype = "i32"
 
                     logger.debug("Output dtype: %s", output_dtype)
-                    preds = self._parse_cairo_response(serialized_output, output_dtype)
+                    preds = self._parse_cairo_response(
+                        serialized_output, output_dtype, model_category
+                    )
+
                 elif self.framework == Framework.EZKL:
                     preds = np.array(serialized_output[0])
                 return (preds, request_id)
             # Here we are returning different things, Tuple vs np.ndarray
             # TODO: make it consistent
             else:
                 if self.session is None:
                     raise ValueError("Session is not initialized.")
                 if input_feed is None:
                     raise ValueError("Input feed is none")
                 preds = self.session.run(None, input_feed)[0]
-                return preds
+                return (preds, None)
         except Exception as e:
             logger.error(f"An error occurred in predict: {e}")
             raise e
 
-    def _format_inputs_for_framework(self, *args, **kwargs):
+    def _format_inputs_for_framework(self, *args: Any, **kwargs: Any) -> Any:
         """
         Formats the inputs for a prediction request for a specific framework.
 
         Args:
             *args: Variable length argument list.
             **kwargs: Arbitrary keyword arguments.
         """
@@ -311,47 +348,58 @@
                 # This should never happen
                 raise ValueError(f"Unsupported framework: {self.framework}")
 
     def _format_inputs_for_cairo(
         self,
         input_file: Optional[str],
         input_feed: Optional[Dict],
-        fp_impl,
+        fp_impl: str,
+        model_category: str,
         job_size: str,
-    ):
+    ) -> Dict[str, str]:
         """
-        Formats the inputs for a prediction request for OrionRunner.
+        Formats the inputs for a prediction request using OrionRunner.
 
-        Args:
-            input_file (Optional[str]): The path to the input file for prediction. Defaults to None.
-            input_feed (Optional[Dict]): A dictionary containing the input data for prediction. Defaults to None.
-            fp_impl (str): The fixed point implementation to use.
+        Parameters:
+            input_file (Optional[str]): Path to the input file for prediction.
+            input_feed (Optional[Dict]): Dictionary containing the input data for prediction.
+            fp_impl (str): The fixed point implementation to be used.
+            model_category (str): The category of the model, which can be one of 'ONNX_ORION', 'XGB', or 'LGBM'.
+            job_size (str): Description or identifier for the size of the job.
 
         Returns:
-            dict: A dictionary representing the formatted inputs for the Cairo prediction request.
+            Dict: A dictionary representing the formatted inputs for the Cairo prediction request.
         """
-        serialized = []
+        formatted_args = []
 
-        if input_file is not None:
-            serialized = serialize(input_file, fp_impl)
+        if input_file:
+            formatted_args.append(serialize(input_file, model_category))
 
-        if input_feed is not None:
-            for name in input_feed:
-                value = input_feed[name]
+        if input_feed:
+            for name, value in input_feed.items():
                 if isinstance(value, np.ndarray):
-                    tensor = create_tensor_from_array(value, fp_impl)
-                    serialized.append(serializer(tensor))
-                else:
-                    serialized.append(serializer(tensor))
+                    if model_category == "ONNX_ORION":
+                        tensor = create_tensor_from_array(value, fp_impl)
+                    elif model_category in ["XGB", "LGBM"]:
+                        tensor = value * 100000
+                        tensor = tensor.astype(np.int64)
+                    else:
+                        tensor = create_tensor_from_array(value, "FP16x16")
+                    formatted_args.append(serializer(tensor))
 
-        return {"job_size": job_size, "args": " ".join(serialized)}
+        return {"job_size": job_size, "args": " ".join(formatted_args)}
 
     def _format_inputs_for_ezkl(
-        self, input_file: str, input_feed: Dict, job_size: str, *args, **kwargs
-    ):
+        self,
+        input_file: str,
+        input_feed: Dict,
+        job_size: str,
+        *args: Any,
+        **kwargs: Any,
+    ) -> Dict[str, Any]:
         """
         Formats the inputs for a prediction request for EZKL.
 
         Args:
             input_file (str): The path to the input file for prediction.
             input_feed (Dict): A dictionary containing the input data for prediction.
 
@@ -370,51 +418,60 @@
                     data = input_feed.reshape([-1])
                 case _:
                     raise ValueError(
                         "Invalid input_feed format. Must be a dictionary with 'input_data' containintg the data array."
                     )
         return {"input_data": [data], "job_size": job_size}
 
-    def _parse_cairo_response(self, response, data_type: str):
+    def _parse_cairo_response(
+        self, response: str, data_type: str, model_category: str
+    ) -> str:
         """
         Parses the response from a OrionRunner prediction request.
 
         Args:
             response (str): The serialized response from the Cairo prediction request.
             data_type (str): The data type to which the response should be deserialized.
             fp_impl (str): The fixed point implementation used.
 
         Returns:
             The deserialized prediction result.
         """
-        return deserialize(response, data_type)
+        return deserialize(response, data_type, framework=model_category)
 
-    def _get_output_dtype(self):
+    def _get_output_dtype(self) -> Optional[str]:
         """
         Retrieve the Cairo output data type base on the operator type of the final node.
 
         Returns:
             The output dtype as a string.
         """
 
-        file = self.version_client.download_original(
-            self.model.id, self.version.version
-        )
+        self._download_model()
+
+        if self._output_path in self._cache:
+            file_path = Path(self._cache.get(self._output_path))
+            with open(file_path, "rb") as f:
+                file = f.read()
 
         model = onnx.load_model_from_string(file)
         graph = model.graph
         output_tensor_name = graph.output[0].name
 
-        def find_producing_node(graph, tensor_name):
+        def find_producing_node(
+            graph: onnx.GraphProto, tensor_name: str
+        ) -> Optional[onnx.NodeProto]:
             for node in graph.node:
                 if tensor_name in node.output:
                     return node
             return None
 
         final_node = find_producing_node(graph, output_tensor_name)
+        if final_node is None:
+            return None
         optype = final_node.op_type
 
         match optype:
             case "TreeEnsembleClassifier":
                 return "(Span<u32>, MutMatrix<FP16x16>)"
 
             case "TreeEnsembleRegressor":
```

### Comparing `giza_actions-0.3.1/giza_actions/utils.py` & `giza_actions-0.3.2/giza_actions/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import json
 import logging
+from typing import Optional
 
 import requests
 from giza import API_HOST
 from giza.client import EndpointsClient, WorkspaceClient
 
 logger = logging.getLogger(__name__)
 
 
-def get_workspace_uri():
+def get_workspace_uri() -> str:
     """
     Retrieves the URI of the current workspace.
 
     This function creates a WorkspaceClient instance using the API_HOST and
     calls its get method to retrieve the current workspace. It then returns
     the URL of the workspace.
 
@@ -21,21 +22,21 @@
     """
     client = WorkspaceClient(API_HOST)
     try:
         workspace = client.get()
     except requests.exceptions.RequestException:
         logger.error("Failed to retrieve workspace")
         logger.error(
-            "Please check that you have created a workspaces using the Giza CLI"
+            "Please check that you have create a workspaces using the Giza CLI"
         )
         raise
     return workspace.url
 
 
-def get_endpoint_uri(model_id: int, version_id: int):
+def get_endpoint_uri(model_id: int, version_id: int) -> Optional[str]:
     """
     Get the deployment URI associated with a specific model and version.
 
     Args:
         model_id (int): The ID of the model.
         version_id (int): The ID of the version.
 
@@ -53,15 +54,15 @@
 
     if len(deployments_list.root) == 1:
         return deployments_list.root[0].uri
     else:
         return None
 
 
-def read_json(file_path: str):
+def read_json(file_path: str) -> dict:
     """
     Read the JSON file from the specified path and return the
     JSON data.
 
     Args:
         file_path (str): The path to the JSON file.
```

### Comparing `giza_actions-0.3.1/pyproject.toml` & `giza_actions-0.3.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "giza-actions"
-version = "0.3.1"
+version = "0.3.2"
 
 description = "A Python SDK for Giza platform"
 authors = [
     "Francisco Algaba <fran@gizatech.xyz>",
     "Raphael Doukhan <raphael@gizatech.xyz>",
     "Gonzalo Mellizo-Soto <gonzalo@gizatech.xyz>"]
 readme = "README.md"
@@ -19,18 +19,19 @@
 httpx = "^0.25.1"
 onnxruntime = "^1.16.3"
 prefect-gcp = "^0.5.4"
 pyyaml = "^6.0.1"
 prefect-docker = "^0.4.1"
 distlib = "^0.3.8"
 giza-cli = ">=0.15.0,<1.0.0"
-giza-osiris = ">=0.2.6,<1.0.0"
+giza-osiris = ">=0.2.8,<1.0.0"
 loguru = "^0.7.2"
 eth-ape = {version = "^0.7.10", optional = true }
 ape-etherscan = {version = "^0.7.2", optional = true }
+diskcache = "^5.6.3"
 
 [tool.poetry.extras]
 agents = ["eth-ape", "ape-etherscan"]
 
 [tool.poetry.dev-dependencies]
 pytest = "^6.2.5"
```

### Comparing `giza_actions-0.3.1/PKG-INFO` & `giza_actions-0.3.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: giza-actions
-Version: 0.3.1
+Version: 0.3.2
 Summary: A Python SDK for Giza platform
 License: MIT
 Author: Francisco Algaba
 Author-email: fran@gizatech.xyz
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: agents
 Requires-Dist: ape-etherscan (>=0.7.2,<0.8.0) ; extra == "agents"
+Requires-Dist: diskcache (>=5.6.3,<6.0.0)
 Requires-Dist: distlib (>=0.3.8,<0.4.0)
 Requires-Dist: eth-ape (>=0.7.10,<0.8.0) ; extra == "agents"
 Requires-Dist: giza-cli (>=0.15.0,<1.0.0)
-Requires-Dist: giza-osiris (>=0.2.6,<1.0.0)
+Requires-Dist: giza-osiris (>=0.2.8,<1.0.0)
 Requires-Dist: httpx (>=0.25.1,<0.26.0)
 Requires-Dist: loguru (>=0.7.2,<0.8.0)
 Requires-Dist: numpy (>=1.26.2,<2.0.0)
 Requires-Dist: onnx (>=1.15.0,<2.0.0)
 Requires-Dist: onnxruntime (>=1.16.3,<2.0.0)
 Requires-Dist: prefect (==2.14.6)
 Requires-Dist: prefect-docker (>=0.4.1,<0.5.0)
```

