# Comparing `tmp/cerebrium-1.19.1-py3-none-any.whl.zip` & `tmp/cerebrium-1.20.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,32 +1,32 @@
-Zip file size: 69300 bytes, number of entries: 30
+Zip file size: 69164 bytes, number of entries: 30
 -rw-r--r--  2.0 unx      134 b- defN 80-Jan-01 00:00 cerebrium/__init__.py
--rw-r--r--  2.0 unx    16818 b- defN 80-Jan-01 00:00 cerebrium/api.py
+-rw-r--r--  2.0 unx    16864 b- defN 80-Jan-01 00:00 cerebrium/api.py
 -rw-r--r--  2.0 unx     9658 b- defN 80-Jan-01 00:00 cerebrium/commands/app.py
 -rw-r--r--  2.0 unx     4419 b- defN 80-Jan-01 00:00 cerebrium/commands/auth.py
--rw-r--r--  2.0 unx     7820 b- defN 80-Jan-01 00:00 cerebrium/commands/config.py
--rw-r--r--  2.0 unx    35925 b- defN 80-Jan-01 00:00 cerebrium/commands/cortex.py
+-rw-r--r--  2.0 unx     7923 b- defN 80-Jan-01 00:00 cerebrium/commands/config.py
+-rw-r--r--  2.0 unx    29130 b- defN 80-Jan-01 00:00 cerebrium/commands/cortex.py
 -rw-r--r--  2.0 unx     2182 b- defN 80-Jan-01 00:00 cerebrium/commands/project.py
--rw-r--r--  2.0 unx    23620 b- defN 80-Jan-01 00:00 cerebrium/commands/serve.py
+-rw-r--r--  2.0 unx    23724 b- defN 80-Jan-01 00:00 cerebrium/commands/serve.py
 -rw-r--r--  2.0 unx     2953 b- defN 80-Jan-01 00:00 cerebrium/commands/storage.py
 -rw-r--r--  2.0 unx      824 b- defN 80-Jan-01 00:00 cerebrium/constants.py
 -rw-r--r--  2.0 unx      826 b- defN 80-Jan-01 00:00 cerebrium/core.py
--rw-r--r--  2.0 unx    16629 b- defN 80-Jan-01 00:00 cerebrium/datatypes.py
+-rw-r--r--  2.0 unx    17254 b- defN 80-Jan-01 00:00 cerebrium/datatypes.py
 -rw-r--r--  2.0 unx     5228 b- defN 80-Jan-01 00:00 cerebrium/local_api_server.py
 -rwxr-xr-x  2.0 unx     1383 b- defN 80-Jan-01 00:00 cerebrium/main.py
 -rw-r--r--  2.0 unx      261 b- defN 80-Jan-01 00:00 cerebrium/utils/__init__.py
 -rw-r--r--  2.0 unx     2514 b- defN 80-Jan-01 00:00 cerebrium/utils/config.py
 -rw-r--r--  2.0 unx     6188 b- defN 80-Jan-01 00:00 cerebrium/utils/display.py
 -rw-r--r--  2.0 unx     2546 b- defN 80-Jan-01 00:00 cerebrium/utils/files.py
 -rw-r--r--  2.0 unx     6800 b- defN 80-Jan-01 00:00 cerebrium/utils/logging.py
 -rw-r--r--  2.0 unx     7693 b- defN 80-Jan-01 00:00 cerebrium/utils/misc.py
 -rw-r--r--  2.0 unx     4505 b- defN 80-Jan-01 00:00 cerebrium/utils/requirements.py
--rw-r--r--  2.0 unx     9925 b- defN 80-Jan-01 00:00 cerebrium/utils/sync_files.py
+-rw-r--r--  2.0 unx    10069 b- defN 80-Jan-01 00:00 cerebrium/utils/sync_files.py
 -rw-r--r--  2.0 unx     8988 b- defN 80-Jan-01 00:00 cerebrium/utils/tomls.py
 -rw-r--r--  2.0 unx     1444 b- defN 80-Jan-01 00:00 cerebrium/utils/watchdog.py
 -rw-r--r--  2.0 unx     2096 b- defN 80-Jan-01 00:00 cerebrium/verification.py
--rw-r--r--  2.0 unx    34594 b- defN 80-Jan-01 00:00 cerebrium-1.19.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     3074 b- defN 80-Jan-01 00:00 cerebrium-1.19.1.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 cerebrium-1.19.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       48 b- defN 80-Jan-01 00:00 cerebrium-1.19.1.dist-info/entry_points.txt
-?rw-r--r--  2.0 unx     2453 b- defN 16-Jan-01 00:00 cerebrium-1.19.1.dist-info/RECORD
-30 files, 221636 bytes uncompressed, 65398 bytes compressed:  70.5%
+-rw-r--r--  2.0 unx    34594 b- defN 80-Jan-01 00:00 cerebrium-1.20.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3025 b- defN 80-Jan-01 00:00 cerebrium-1.20.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 cerebrium-1.20.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       48 b- defN 80-Jan-01 00:00 cerebrium-1.20.0.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx     2454 b- defN 16-Jan-01 00:00 cerebrium-1.20.0.dist-info/RECORD
+30 files, 215815 bytes uncompressed, 65262 bytes compressed:  69.8%
```

## zipnote {}

```diff
@@ -69,23 +69,23 @@
 
 Filename: cerebrium/utils/watchdog.py
 Comment: 
 
 Filename: cerebrium/verification.py
 Comment: 
 
-Filename: cerebrium-1.19.1.dist-info/LICENSE
+Filename: cerebrium-1.20.0.dist-info/LICENSE
 Comment: 
 
-Filename: cerebrium-1.19.1.dist-info/METADATA
+Filename: cerebrium-1.20.0.dist-info/METADATA
 Comment: 
 
-Filename: cerebrium-1.19.1.dist-info/WHEEL
+Filename: cerebrium-1.20.0.dist-info/WHEEL
 Comment: 
 
-Filename: cerebrium-1.19.1.dist-info/entry_points.txt
+Filename: cerebrium-1.20.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: cerebrium-1.19.1.dist-info/RECORD
+Filename: cerebrium-1.20.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cerebrium/api.py

```diff
@@ -417,22 +417,25 @@
             cerebrium_log(
                 level="ERROR",
                 message="Error streaming logs. Please check your internet connection and ensure you are logged in. If this issue persists, please contact support.",
             )
             exit()
 
         if response.status_code == 200:
-            for line in response.iter_lines():
-                if stop_event.is_set():  # Check if the stop event is set
-                    break  # Exit the loop if the stop event is set
-                if line:
-                    decoded_line = line.decode("utf-8")
-                    log.log_formatted_response(decoded_line)
-                    if not start_event.is_set():
-                        start_event.set()
+            iterator = response.iter_lines()
+            while not stop_event.is_set():
+                try:
+                    line = next(iterator)
+                    if line:
+                        decoded_line = line.decode("utf-8")
+                        log.log_formatted_response(decoded_line)
+                        if not start_event.is_set():
+                            start_event.set()
+                except StopIteration:
+                    break
         else:
             if not stop_event.is_set():
                 log.logger.error(
                     f"Failed to stream logs. Status code: {response.status_code}"
                 )
     except Exception as e:
         log.logger.error(f"An error occurred while streaming logs: {e}")
```

## cerebrium/commands/config.py

```diff
@@ -74,22 +74,25 @@
     gpu: Annotated[
         str,
         typer.Option(
             help=(
                 "Hardware to use for the Cortex deployment. "
                 "Defaults to 'AMPERE_A10'. "
                 "Can be one of "
-                "'AMPERE_A10'"
-                "'ADA_L4'"
-                "'TURING_4000', "
-                "'TURING_5000', "
-                "'AMPERE_A4000', "
-                "'AMPERE_A5000', "
-                "'AMPERE_A6000', "
-                "'AMPERE_A100'"
+                "'AMPERE_A10', "
+                "'ADA_L4', "
+                "'TURING_T4', "
+                "'INF2', "
+                "'TRN1', "
+                # "'TURING_4000', "
+                # "'TURING_5000', "
+                # "'AMPERE_A4000', "
+                # "'AMPERE_A5000', "
+                # "'AMPERE_A6000', "
+                # "'AMPERE_A100'."
             ),
         ),
     ] = "",
     cpu: Annotated[
         Optional[int],
         typer.Option(
             min=MIN_CPU,
```

## cerebrium/commands/cortex.py

```diff
@@ -28,28 +28,17 @@
 from cerebrium.utils import logging
 from cerebrium.utils.config import archive_file, update_config_from_files
 from cerebrium.utils.logging import cerebrium_log
 from cerebrium.utils.misc import get_function_params
 from cerebrium.utils.sync_files import upload_files_to_s3, upload_marker_file_and_delete
 
 _EXAMPLE_MAIN = """
-from typing import Optional
-from pydantic import BaseModel
-
-
-class Item(BaseModel):
-    prompt: str
-    your_param: Optional[str] = None # an example optional parameter
-
-
-def predict(item, run_id, logger):
-    item = Item(**item)
-
-    my_results = {"prediction": item.prompt, "your_optional_param": item.your_param}
-    my_status_code = 200 # if you want to return some status code
+def run(param_1: str, param_2: str, run_id):  # run_id is optional, injected by Cerebrium at runtime
+    my_results = {"1": param_1, "2": param_2}
+    my_status_code = 200 # if you want to return a specific status code
 
     return {"my_result": my_results, "status_code": my_status_code} # return your results
 """
 
 
 def was_provided(param_name: str, param_value: Any, defaults: Dict[str, Any]) -> bool:
     """Check if a parameter was explicitly provided by comparing against its default value."""
@@ -206,17 +195,17 @@
         name = name.lower()
 
     print(f"Initializing Cerebrium Cortex project in {init_dir}")
     pip = (
         pip
         if pip
         else (
-            "['transformers', 'torch>=2.0.0', 'pydantic']"
+            "['transformers', 'torch>=2.0.0']"
             if cuda_version == "12"
-            else "['transformers', 'torch<2.0.0', 'pydantic']"
+            else "['transformers', 'torch<2.0.0']"
         )
     )
 
     if not os.path.exists(init_dir):
         os.makedirs(init_dir)
     elif os.listdir(init_dir) and not overwrite:
         cerebrium_log(
@@ -283,22 +272,27 @@
         Optional[bool], typer.Option(help="Flag to disable syntax check.")
     ] = None,
     gpu: Annotated[
         Optional[str],
         typer.Option(
             help=(
                 "Hardware to use for the Cortex deployment. "
-                "Defaults to 'AMPERE_A6000'. "
+                "Defaults to 'AMPERE_A10'. "
                 "Can be one of "
-                "'TURING_4000', "
-                "'TURING_5000', "
-                "'AMPERE_A4000', "
-                "'AMPERE_A5000', "
-                "'AMPERE_A6000', "
-                "'AMPERE_A100'"
+                # "'TURING_4000', "
+                # "'TURING_5000', "
+                # "'AMPERE_A4000', "
+                # "'AMPERE_A5000', "
+                # "'AMPERE_A6000', "
+                # "'AMPERE_A100', "
+                # "'AMPERE_A10', "
+                "'ADA_L4', "
+                "'TURING_T4', "
+                "'INF2', "
+                "'TRN1'"
             ),
         ),
     ] = None,
     cpu: Annotated[
         Optional[int],
         typer.Option(
             min=constants.MIN_CPU,
@@ -495,32 +489,34 @@
         scaling=datatypes.CerebriumScaling(**config_obj["scaling"]),
         build=datatypes.CerebriumBuild(**config_obj["build"]),
         deployment=datatypes.CerebriumDeployment(**config_obj["deployment"]),
         hardware=datatypes.CerebriumHardware(**config_obj["hardware"]),
         dependencies=datatypes.CerebriumDependencies(**config_obj["dependencies"]),
         cerebrium_version=cerebrium_version,
     )
+    # Check if the provider is Coreweave, if so print a V3 deprecation warning
+    if cerebrium_config.hardware.provider == "coreweave":
+        cerebrium_log(
+            message="WARNING: Cortex V4 does not currently support Coreweave. Please considering updating your deployment to V4 and deploying to AWS.",
+            level="WARNING",
+        )
 
     build_status, setup_response = package_app(
         cerebrium_config, datatypes.OperationType.DEPLOY
     )
     if setup_response is None:
         cerebrium_log(
             message="Error setting up your deployment and getting your logs. Please check your dashboard or contact support if the issue persists.",
             color="red",
         )
         sys.exit(1)
     if "success" == build_status:
         project_id = setup_response["projectId"]
         jwt = setup_response["jwt"]
-
-        if constants.env == "prod":
-            endpoint = f"https://run.cerebrium.ai/v3/{project_id}/{cerebrium_config.deployment.name}/predict"
-        else:
-            endpoint = f"https://dev-run.cerebrium.ai/v3/{project_id}/{cerebrium_config.deployment.name}/predict"
+        endpoint = setup_response["internalEndpoint"]
 
         dashboard_url = f"{api.dashboard_url}/projects/{project_id}/models/{project_id}-{cerebrium_config.deployment.name}"
 
         info_string = (
             f"🔗 [link={dashboard_url}]View your deployment dashboard here[/link]\n"
             f"🔗 [link={dashboard_url}?tab=builds]View builds here[/link]\n"
             f"🔗 [link={dashboard_url}?tab=runs]View runs here[/link]\n\n"
@@ -534,18 +530,18 @@
             width=100,
             padding=(1, 2),
         )
 
         console(Group(dashboard_info))
 
         curl_command = colored(
-            f"curl -X POST {endpoint} \\\n"
+            f"curl -X POST {endpoint}/{{function}} \\\n"
             "     -H 'Content-Type: application/json'\\\n"
-            f"     -H 'Authorization: {jwt}'\\\n"
-            '     --data \'{"prompt": "Hello World!"}\'',
+            f"     -H 'Authorization: Bearer {jwt}'\\\n"
+            '     --data \'{"param": "Hello World!"}\'',
             "green",
         )
         print(
             "\n💡You can call the endpoint with the following curl command:\n"
             f"{curl_command}"
         )
     elif build_status in ["build_failure", "init_failure"]:
@@ -553,208 +549,14 @@
             Text(
                 "Unfortunately there was an issue with your deployment",
                 style="red",
             )
         )
 
 
-@cli.command("build")
-def build(
-    name: Annotated[str, typer.Option(help="Name of the Cortex deployment.")] = "",
-    disable_syntax_check: Annotated[
-        bool, typer.Option(help="Flag to disable syntax check.")
-    ] = False,
-    gpu: Annotated[
-        Optional[str],
-        typer.Option(
-            help=(
-                "Hardware to use for the Cortex deployment. "
-                "Defaults to 'AMPERE_A6000'. "
-                "Can be one of "
-                "'TURING_4000', "
-                "'TURING_5000', "
-                "'AMPERE_A4000', "
-                "'AMPERE_A5000', "
-                "'AMPERE_A6000', "
-                "'AMPERE_A100'"
-            ),
-        ),
-    ] = None,
-    cpu: Annotated[
-        Optional[int],
-        typer.Option(
-            min=constants.MIN_CPU,
-            max=constants.MAX_CPU,
-            help=(
-                "Number of vCPUs to use for the Cortex deployment. Defaults to 2. "
-                "Can be an integer between 1 and 48."
-            ),
-        ),
-    ] = None,
-    memory: Annotated[
-        Optional[float],
-        typer.Option(
-            min=constants.MIN_MEMORY,
-            max=constants.MAX_MEMORY,
-            help=(
-                "Amount of memory(GB) to use for the Cortex deployment. Defaults to {constants.DEFAULT_MEMORY}. "
-                "Can be a float between 2.0 and 256.0 depending on hardware selection."
-            ),
-        ),
-    ] = None,
-    gpu_count: Annotated[
-        Optional[int],
-        typer.Option(
-            min=1,
-            max=constants.MAX_GPU_COUNT,
-            help=(
-                "Number of GPUs to use for the Cortex deployment. Defaults to {constants.DEFAULT_GPU_COUNT}. "
-                "Can be an integer between 1 and 8."
-            ),
-        ),
-    ] = None,
-    python_version: Annotated[
-        Optional[str],
-        typer.Option(
-            help=(
-                "Python version to use. "
-                "Currently, we support '3.8' to '3.11'. Defaults to '{constants.PYTHON_VERSION}'"
-            ),
-        ),
-    ] = None,
-    predict: Annotated[
-        Optional[str],
-        typer.Option(
-            help="JSON string containing all the parameters that will be used to run your "
-            "deployment's predict function on build to ensure your new deployment will work "
-            "as expected before replacing your existing deployment.",
-        ),
-    ] = None,
-    include: Annotated[
-        Optional[str],
-        typer.Option(
-            help=(
-                "Comma delimited string list of relative paths to files/folder to include. "
-                "Defaults to all visible files/folders in project root."
-            ),
-        ),
-    ] = None,
-    exclude: Annotated[
-        Optional[str],
-        typer.Option(
-            help="Comma delimited string list of relative paths to files/folder to exclude. Defaults to all hidden files/folders in project root.",
-        ),
-    ] = None,
-    force_rebuild: Annotated[Optional[bool], typer.Option()] = False,
-    config_file: Annotated[
-        Optional[str],
-        typer.Option(
-            help="Path to cerebrium.toml file. You can generate a config using `cerebrium init-cortex`. The contents of the deployment config file are overridden by the command line arguments.",
-        ),
-    ] = None,
-    log_level: Annotated[
-        Optional[str],
-        typer.Option(
-            help="Log level for the Cortex build. Can be one of 'DEBUG' or 'INFO'"
-        ),
-    ] = "",
-    disable_confirmation: Annotated[
-        Optional[bool],
-        typer.Option(
-            "--disable-confirmation",
-            "-q",
-            "-y",
-            help="Whether to disable the confirmation prompt before deploying.",
-        ),
-    ] = None,
-    disable_predict: Annotated[
-        Optional[bool], typer.Option(help="Flag to disable running predict function.")
-    ] = None,
-    disable_animation: Annotated[
-        Optional[bool],
-        typer.Option(
-            help="Whether to use TQDM and yaspin animations.",
-        ),
-    ] = None,
-    disable_build_logs: Annotated[
-        Optional[bool],
-        typer.Option(help="Whether to disable build logs during a deployment."),
-    ] = None,
-    hide_public_endpoint: Annotated[
-        Optional[bool],
-        typer.Option(
-            help="Whether to hide the public endpoint of the deployment when printing the logs.",
-        ),
-    ] = None,
-    cuda_version: Annotated[
-        Optional[str],
-        typer.Option(
-            help=(
-                "CUDA version to use. "
-                "Currently, we support 11.8 as '11' and 12.2 as '12'. Defaults to '12'"
-            ),
-        ),
-    ] = None,
-    provider: Annotated[
-        Optional[str],
-        typer.Option(
-            help=f"Provider to deploy to. Can be one of: 'aws' or 'coreweave'. This is auto-populated if left unspecified"
-        ),
-    ] = None,
-    region: Annotated[
-        Optional[str],
-        typer.Option(
-            help=f"Region to deploy to. Can be one of: 'us-east-1' or 'us-central-1'. This is auto-populated if left unspecified"
-        ),
-    ] = None,
-):
-    """
-    Build and run your Cortex files on Cerebrium to verify that they're working as expected.
-    """
-    if config_file is None or not config_file.strip():
-        config_file = "cerebrium.toml"
-
-    # func_defaults contains all parameters with their default values
-    func_defaults = {
-        k: v.default
-        for k, v in inspect.signature(deploy).parameters.items()
-        if v.default is not inspect.Parameter.empty
-    }
-    # provided_params only include explicitly provided parameters
-    provided_params = {
-        param: value
-        for param, value in locals().items()
-        if param in func_defaults and was_provided(param, value, func_defaults)
-    }
-    # Merge func_defaults with provided_params. Provided values override default values where applicable.
-    final_params = {**func_defaults, **provided_params}
-
-    # load config toml file and merge with param values
-    config_obj = utils.misc.merge_config_with_params("cerebrium.toml", final_params)
-
-    ##validation is done with types in classes
-    cerebrium_config = datatypes.CerebriumConfig(
-        scaling=datatypes.CerebriumScaling(**config_obj["scaling"]),
-        build=datatypes.CerebriumBuild(**config_obj["build"]),
-        deployment=datatypes.CerebriumDeployment(**config_obj["deployment"]),
-        hardware=datatypes.CerebriumHardware(**config_obj["hardware"]),
-        dependencies=datatypes.CerebriumDependencies(**config_obj["dependencies"]),
-        cerebrium_version=cerebrium_version,
-    )
-
-    build_status, _ = package_app(cerebrium_config, datatypes.OperationType.RUN)
-    if "success" in build_status:
-        console(
-            Text(
-                "Unfortunately there was an issue with running your deployment",
-                style="red",
-            )
-        )
-
-
 def package_app(
     cerebrium_config: datatypes.CerebriumConfig, app_type: datatypes.OperationType
 ):
     # Get the files in the users directory
     cerebrium_config.file_list = utils.determine_includes(
         include=cerebrium_config.deployment.include,
         exclude=cerebrium_config.deployment.exclude,
@@ -896,15 +698,14 @@
                 stop_event=stop_event,
                 log_thread=log_thread,
                 is_interrupt=True,
             )
         finally:
             # Stop the Live instance after the loop
             live.stop()
-
         log_thread.join()
     elif build_status == "running":
         print("🤷 No file changes detected. Not fetching logs")
     else:
         if spinner:
             spinner.stop(text="Build failed")
         cerebrium_log("ERROR", "Build failed.")
```

## cerebrium/commands/serve.py

```diff
@@ -51,22 +51,25 @@
         ),
     ] = 7900,
     gpu: Annotated[
         Optional[str],
         typer.Option(
             help=(
                 "Hardware to use for the Cortex deployment. "
-                "Defaults to 'AMPERE_A6000'. "
+                "Defaults to 'AMPERE_A10'. "
                 "Can be one of "
-                "'TURING_4000', "
-                "'TURING_5000', "
-                "'AMPERE_A4000', "
-                "'AMPERE_A5000', "
-                "'AMPERE_A6000', "
-                "'AMPERE_A100'"
+                "'AMPERE_A10', "
+                "'ADA_L4', "
+                "'TURING_T4', "
+                # "'TURING_4000', "
+                # "'TURING_5000', "
+                # "'AMPERE_A4000', "
+                # "'AMPERE_A5000', "
+                # "'AMPERE_A6000', "
+                # "'AMPERE_A100'"
             ),
         ),
     ] = None,
     cpu: Annotated[
         Optional[int],
         typer.Option(
             min=constants.MIN_CPU,
```

## cerebrium/datatypes.py

```diff
@@ -231,23 +231,50 @@
         max_memory=124.0,
         max_cpu=30,
         VRAM=24,
         has_nvlink=False,
         gpu_model="A10",
         provider_names=["aws"],
     )
+    TURING_T4: Hardware = Hardware(
+        name="TURING_T4",
+        max_memory=124.0,
+        max_cpu=30,
+        VRAM=24,
+        has_nvlink=False,
+        gpu_model="T4",
+        provider_names=["aws"],
+    )
     ADA_L4: Hardware = Hardware(
         name="ADA_L4",
         max_memory=16.0,
         max_cpu=4,
         VRAM=24,
         has_nvlink=False,
         gpu_model="L4",
         provider_names=["aws"],
     )
+    INF2: Hardware = Hardware(
+        name="INF2",
+        max_memory=384.0,
+        max_cpu=6,
+        VRAM=192,
+        has_nvlink=False,
+        gpu_model="inf2",
+        provider_names=["aws"],
+    )
+    TRN1: Hardware = Hardware(
+        name="TRN1",
+        max_memory=512.0,
+        max_cpu=128,
+        VRAM=512,
+        has_nvlink=False,
+        gpu_model="trn1",
+        provider_names=["aws"],
+    )
 
     @classmethod
     def available_hardware(cls):
         return list(cls.__annotations__.keys())
 
 
 class CerebriumScaling:
```

## cerebrium/utils/sync_files.py

```diff
@@ -71,23 +71,25 @@
     """Function to upload a single file."""
 
     try:
         if os.stat(file_path).st_size == 0:
             upload_response = requests.put(upload_url, data=b"")
         else:
             with open(file_path, "rb") as file:
+                # file.seek(0)  # reset file to beginning for each read
                 wrapped_file = (
                     CallbackIOWrapper(pbar.update, file, "read") if pbar else file
                 )
                 upload_response = requests.put(
                     upload_url,
                     data=wrapped_file,  # type: ignore
                     timeout=60,
                     stream=True,
                 )
+                # file.seek(0)  # reset file to beginning for next read
         if upload_response.status_code != 200:
             raise Exception(
                 f"Failed to upload {file_name}. Status code: {upload_response.status_code}"
             )
         return 1
     except Exception as e:
         print(f"Error uploading {file_name}: {e}")
```

## Comparing `cerebrium-1.19.1.dist-info/LICENSE` & `cerebrium-1.20.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `cerebrium-1.19.1.dist-info/METADATA` & `cerebrium-1.20.0.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: cerebrium
-Version: 1.19.1
+Version: 1.20.0
 Summary: 
 License: AGPL-3.0-only
 Author: Elijah Roussos
 Author-email: elijah@cerebrium.ai
-Requires-Python: >=3.9,<3.13
+Requires-Python: >=3.10,<3.13
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: aiofiles (>=23.2.1,<24.0.0)
 Requires-Dist: fastapi (>=0.109.2,<0.110.0)
 Requires-Dist: loguru (>=0.7)
 Requires-Dist: pyflakes (>=3.1.0,<4.0.0)
```

## Comparing `cerebrium-1.19.1.dist-info/RECORD` & `cerebrium-1.20.0.dist-info/RECORD`

 * *Files 17% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 cerebrium/__init__.py,sha256=2iYsq4NIdrDhDHFU-3FXZIpZSVzTdgGehXDHfBBMg4o,134
-cerebrium/api.py,sha256=C5qDrdUqMP4OowLGSWmhUujzR5LphPaxBIC1auDJr20,16818
+cerebrium/api.py,sha256=-f00NLJaqnSjjiKnxP6jSf5yS7w_uGk5QUxk10t-UZI,16864
 cerebrium/commands/app.py,sha256=O4DMFEd0DrgonLrMb-V-Zi_9S31C30TKqCBn6myCJzc,9658
 cerebrium/commands/auth.py,sha256=FBniarlqgLz69UXdf2wCf2z63tXQbtF6T9CGOC8lm-4,4419
-cerebrium/commands/config.py,sha256=Pk2eS4zK3dr3GxlRyowrxyiLc6ntMmKCtezvPzcjRT8,7820
-cerebrium/commands/cortex.py,sha256=wMVytwJAKqOa_V_VoZMLX3Fg4VZOp3uH2u42AsksUOQ,35925
+cerebrium/commands/config.py,sha256=2zzfgWgPJZCWziceSP0D3EIKRwjZjx0aqkvBJ8cRoCY,7923
+cerebrium/commands/cortex.py,sha256=-MalhmDi5fazg7nRH1AFyIk_u1VX5Kn8IGIdRMllwYw,29130
 cerebrium/commands/project.py,sha256=LxOuJw18LOk1pp7xyDt66Ud8VIBO9bCJKfZ7yBfLUWM,2182
-cerebrium/commands/serve.py,sha256=uMT333GeNubvr3WU1oPfq2TYmVpIN6OkV5wNrNjYKAA,23620
+cerebrium/commands/serve.py,sha256=5FPkS6cOZyUnUXb3BycDXJ_Lz6dAkycwBH30RGvUPtg,23724
 cerebrium/commands/storage.py,sha256=-M7Uo1CTj5OT1UX7ymKpuUMRihV69SoMmMPZYC9pvcQ,2953
 cerebrium/constants.py,sha256=rA_gaqPRJNxKdJPlgm5q2b7NAkM8-rYaAMVsws6lSKg,824
 cerebrium/core.py,sha256=uy5xiLHm6ZwL_vWDbW2-soOfo05Vw4hRIuHC-7QFIFQ,826
-cerebrium/datatypes.py,sha256=wmMM-4kyEoGvt7sjPHBgARIXkb3TtZRhGVr5xHeZl4k,16629
+cerebrium/datatypes.py,sha256=5qoRW0pNfhKyVeyJvjmNW6ClGWjHZEbdXWGVEvBzdRo,17254
 cerebrium/local_api_server.py,sha256=5mLBuRzrIYNkO8uTbn8SSO_98WTKoEny4GC8XWTIzVc,5228
 cerebrium/main.py,sha256=8jLEDSGu4mhSmGaM4Y4-U5crAJ1MQcyqR5wbOpJH5mY,1383
 cerebrium/utils/__init__.py,sha256=Yid6nw5wQWUFBOvlQ_JFgXJC8BugBiF2D_glpisZpG0,261
 cerebrium/utils/config.py,sha256=rWQaCwzF4f3-vm6Z2eTQYlQ1FyXIlYGr5oGS0aPzyV0,2514
 cerebrium/utils/display.py,sha256=kFHSAl1_rjE77lA83tzrj1aHbimSWnpysSojDUTMiVs,6188
 cerebrium/utils/files.py,sha256=Sv6O8RWIy6OILaFtR4ewzDsdJjEVOBs2hLjP8UMvC-M,2546
 cerebrium/utils/logging.py,sha256=0DJzOH28bAymYfjuUQRyFmi8yWfR7b8sPjk2dp_h-VU,6800
 cerebrium/utils/misc.py,sha256=YfJTheGRHA9QTQr15AI70ujKUhU35NWYlk3EyTOTylI,7693
 cerebrium/utils/requirements.py,sha256=6mrnoqySpuxSRx0U80OMmw9_09l-4P_FS3t2QFvJLEE,4505
-cerebrium/utils/sync_files.py,sha256=nW2PJNjp2sfo19B2dAMhgjCWPEndxSk4OwnJcH_renE,9925
+cerebrium/utils/sync_files.py,sha256=0VrowWvyGwR8IpKn8kESjak7X67kwbqLAamw8JNGjUQ,10069
 cerebrium/utils/tomls.py,sha256=r8kCaJ3CL9JFIbHi3NmX_IED0vS_dT7-oG2SIW5eO14,8988
 cerebrium/utils/watchdog.py,sha256=Kz2DKtLCxnjb_UrMEFgor2_jsG66gTEG24xJcTYTYuE,1444
 cerebrium/verification.py,sha256=UntzxtLnJwZI87BznqmU_dwjp_JCaV14jPbSFQyWWMk,2096
-cerebrium-1.19.1.dist-info/LICENSE,sha256=QoCdyu_al_XTJCs6xphksUTo6SgGRe_y3AnD6oeKziw,34594
-cerebrium-1.19.1.dist-info/METADATA,sha256=SKpRKM348H00gYczZyz_MOu0friPFRsdVFRFR1KXQXA,3074
-cerebrium-1.19.1.dist-info/WHEEL,sha256=sP946D7jFCHeNz5Iq4fL4Lu-PrWrFsgfLXbbkciIZwg,88
-cerebrium-1.19.1.dist-info/entry_points.txt,sha256=X8NSRgq1hWqWRFwDhH1YWLG36V8vpPJpWFHr6jHTwwk,48
-cerebrium-1.19.1.dist-info/RECORD,,
+cerebrium-1.20.0.dist-info/LICENSE,sha256=QoCdyu_al_XTJCs6xphksUTo6SgGRe_y3AnD6oeKziw,34594
+cerebrium-1.20.0.dist-info/METADATA,sha256=EYvS8sheQEL2oY_ABo6cSlzZJyyH1eDBPAba_CJ1G4o,3025
+cerebrium-1.20.0.dist-info/WHEEL,sha256=sP946D7jFCHeNz5Iq4fL4Lu-PrWrFsgfLXbbkciIZwg,88
+cerebrium-1.20.0.dist-info/entry_points.txt,sha256=X8NSRgq1hWqWRFwDhH1YWLG36V8vpPJpWFHr6jHTwwk,48
+cerebrium-1.20.0.dist-info/RECORD,,
```

