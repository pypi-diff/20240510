# Comparing `tmp/kaas_cli-0.1.5.tar.gz` & `tmp/kaas_cli-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kaas_cli-0.1.5.tar", max compression
+gzip compressed data, was "kaas_cli-0.1.6.tar", max compression
```

## Comparing `kaas_cli-0.1.5.tar` & `kaas_cli-0.1.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1073 2024-05-08 20:03:15.593414 kaas_cli-0.1.5/LICENSE
--rw-r--r--   0        0        0     1571 2024-04-04 02:39:44.131953 kaas_cli-0.1.5/README.md
--rw-r--r--   0        0        0     1610 2024-05-10 03:43:51.935668 kaas_cli-0.1.5/pyproject.toml
--rw-r--r--   0        0        0       48 2024-05-08 21:50:45.591034 kaas_cli-0.1.5/src/kaas_cli/__init__.py
--rw-r--r--   0        0        0     1253 2024-03-14 19:47:46.596348 kaas_cli-0.1.5/src/kaas_cli/__main__.py
--rw-r--r--   0        0        0     7407 2024-05-09 18:56:20.700823 kaas_cli-0.1.5/src/kaas_cli/cli.py
--rw-r--r--   0        0        0    23215 2024-05-07 15:47:59.868410 kaas_cli-0.1.5/src/kaas_cli/client.py
--rw-r--r--   0        0        0     1141 2024-05-07 15:47:59.868410 kaas_cli-0.1.5/src/kaas_cli/config.py
--rw-r--r--   0        0        0      945 2024-04-04 02:39:50.272003 kaas_cli-0.1.5/src/kaas_cli/constants.py
--rw-r--r--   0        0        0       58 2024-01-12 17:27:55.752690 kaas_cli-0.1.5/src/kaas_cli/hello.py
--rw-r--r--   0        0        0        0 2024-01-12 17:27:55.752690 kaas_cli-0.1.5/src/kaas_cli/py.typed
--rw-r--r--   0        0        0      346 2024-03-19 20:01:38.753155 kaas_cli-0.1.5/src/kaas_cli/types.py
--rw-r--r--   0        0        0     2464 1970-01-01 00:00:00.000000 kaas_cli-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1073 2024-05-10 21:42:32.832005 kaas_cli-0.1.6/LICENSE
+-rw-r--r--   0        0        0     1639 2024-05-10 21:42:32.832005 kaas_cli-0.1.6/README.md
+-rw-r--r--   0        0        0     1628 2024-05-10 21:42:32.832005 kaas_cli-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0       48 2024-05-10 21:42:32.832005 kaas_cli-0.1.6/src/kaas_cli/__init__.py
+-rw-r--r--   0        0        0     1253 2024-05-10 21:42:32.832005 kaas_cli-0.1.6/src/kaas_cli/__main__.py
+-rw-r--r--   0        0        0     7916 2024-05-10 21:42:32.832005 kaas_cli-0.1.6/src/kaas_cli/cli.py
+-rw-r--r--   0        0        0    23212 2024-05-10 21:42:32.832005 kaas_cli-0.1.6/src/kaas_cli/client.py
+-rw-r--r--   0        0        0     1139 2024-05-10 21:42:32.832005 kaas_cli-0.1.6/src/kaas_cli/config.py
+-rw-r--r--   0        0        0      945 2024-05-10 21:42:32.832005 kaas_cli-0.1.6/src/kaas_cli/constants.py
+-rw-r--r--   0        0        0       58 2024-05-10 21:42:32.832005 kaas_cli-0.1.6/src/kaas_cli/hello.py
+-rw-r--r--   0        0        0        0 2024-05-10 21:42:32.832005 kaas_cli-0.1.6/src/kaas_cli/py.typed
+-rw-r--r--   0        0        0      884 2024-05-10 21:42:32.832005 kaas_cli-0.1.6/src/kaas_cli/types.py
+-rw-r--r--   0        0        0     2571 1970-01-01 00:00:00.000000 kaas_cli-0.1.6/PKG-INFO
```

### Comparing `kaas_cli-0.1.5/LICENSE` & `kaas_cli-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `kaas_cli-0.1.5/README.md` & `kaas_cli-0.1.6/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 ## For Developers
 
 Prerequisites: `python >= 3.10`, `pip >= 20.0.2`, `poetry >= 1.3.2`.
 
 ### Installation
 
-To install the package using `pip`, start by building it:
+To install the package using `pip`, start by building from [Source](https://github.com/runtimeverification/kaas)
 
 ```bash
 make build
 pip install dist/*.whl
 ```
 
 Configure the CLI by copying the example environment file and setting up the necessary environment variables:
@@ -23,24 +23,25 @@
 
 ### Environment Variables
 
 Here's an overview of the environment variables:
 
 - **SERVER_URL**: The KaaS server API address for the main interaction within the CLI tool. This is a required field. For local development, use `http://localhost:5000`.
 - **DEFAULT_DIRECTORY**: The folder path for artifacts. This is an optional field. You can leave it empty.
-- **DEFAULT_PROJECT_ID**: Artifacts should be associated with a project ID. This is an optional field. You can leave it empty.
-- **DEFAULT_TOKEN**: If the user is not the owner of the project, they are required to provide a security token. This is an optional field. You can leave it empty.
+- **DEFAULT_VAULT_ID**: Artifacts should be associated with a project ID. This is an optional field. You can leave it empty.
+- **DEFAULT_KEY**: If the user is not the owner of the project, they are required to provide a security key. This is an optional field. You can leave it empty.
 
 ### Usage
 
 After installing the dependencies with `poetry install`, you can spawn a shell using `poetry shell`, or alternatively, use `make`:
 
 ```bash
 make shell
 kaas-cli hello
+kaas-cli --version
 ```
 
 To verify the installation, run `kaas-cli hello`. If you see the message `Hello World!`, the CLI is set up correctly.
 
 ### Documentation
 
 For detailed usage instructions of the `kaas-cli` tool, please refer to the official [documentation](https://docs.runtimeverification.com/kaas/guides/getting-started).
```

### Comparing `kaas_cli-0.1.5/pyproject.toml` & `kaas_cli-0.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "kaas-cli"
-version = "0.1.5"
+version = "0.1.6"
 description = "Command line utility for K as a Service"
 authors = [
     "Runtime Verification, Inc. <contact@runtimeverification.com>",
 ]
 readme = "README.md"
 
 [tool.poetry.dependencies]
@@ -23,14 +23,15 @@
 pytest-watch = "^4.2.0"
 python-dotenv = "^1.0.1"
 pytest = "^8.0.1"
 jmespath = "^1.0.1"
 types-jmespath = "^1.0.2.20240106"
 requests = "^2.31.0"
 click = "^8.0.1"
+dacite = "^1.8.1"
 
 [tool.poetry.group.dev.dependencies]
 autoflake = "*"
 black = "*"
 flake8 = "*"
 flake8-bugbear = "*"
 flake8-comprehensions = "*"
```

### Comparing `kaas_cli-0.1.5/src/kaas_cli/__main__.py` & `kaas_cli-0.1.6/src/kaas_cli/__main__.py`

 * *Files identical despite different names*

### Comparing `kaas_cli-0.1.5/src/kaas_cli/cli.py` & `kaas_cli-0.1.6/src/kaas_cli/cli.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,26 +1,31 @@
 from __future__ import annotations
 
+import json
+from dataclasses import asdict
 from typing import TYPE_CHECKING
 
 from kaas_cli import __version__
 
 import click
+from dacite import from_dict, Config
 
 from .client import KaasClient
 from .config import DEFAULT_DIRECTORY, DEFAULT_PROJECT_ID, DEFAULT_TOKEN, SERVER_URL, CustomHelpOption
 
 if TYPE_CHECKING:
     from click.core import Context
 
+from .types import Vault, Key
+
 
 @click.group()
 @click.option("--url", "-u", default=SERVER_URL, show_default=True, help="Server URL")
-@click.option("--token", "-t", default=DEFAULT_TOKEN, help="Personal access token for vault")
-@click.option("--vault", "-v", default=DEFAULT_PROJECT_ID, help="Vault hash")
+@click.option("--token", "-t", default=DEFAULT_TOKEN, help="Personal access key for vault")
+@click.option("--vault", "-v", default=DEFAULT_PROJECT_ID, help="Vault ID")
 @click.version_option(version=__version__, prog_name='kaas-cli')
 @click.pass_context
 def cli(ctx: Context, url: str, token: str | None, vault: str | None) -> None:
     """KaaS Command Line Interface"""
     ctx.ensure_object(dict)
     ctx.obj["client"] = KaasClient(url=url, token=token, vault=vault)
 
@@ -31,16 +36,16 @@
     "--directory",
     default=DEFAULT_DIRECTORY,
     show_default=True,
     type=click.Path(exists=True, file_okay=False, dir_okay=True),
     help="Directory containing proofs to upload",
 )
 @click.option("--url", "-u", default=SERVER_URL, show_default=True, help="Server URL")
-@click.option("--token", "-t", default=DEFAULT_TOKEN, help="Personal access token for vault")
-@click.option("--vault", "-v", default=DEFAULT_PROJECT_ID, help="Vault hash")
+@click.option("--token", "-t", default=DEFAULT_TOKEN, help="Personal access key for vault")
+@click.option("--vault", "-v", default=DEFAULT_PROJECT_ID, help="Vault ID")
 @click.pass_context
 def upload(ctx: Context, directory: str, url: str | None, token: str | None, vault: str | None) -> None:
     ctx.ensure_object(dict)
     client: KaasClient = KaasClient(url=url, token=token, vault=vault)
     ctx.obj["client"] = client
     response_message = client.upload_files_s3(directory=directory)
     click.echo(response_message)
@@ -52,16 +57,16 @@
     "--directory",
     default=DEFAULT_DIRECTORY,
     show_default=True,
     type=click.Path(exists=False, file_okay=False, dir_okay=True),
     help="Directory to save downloaded proofs",
 )
 @click.option("--url", "-u", default=SERVER_URL, show_default=True, help="Server URL")
-@click.option("--token", "-t", default=DEFAULT_TOKEN, help="Personal access token for vault")
-@click.option("--vault", "-v", default=DEFAULT_PROJECT_ID, help="Vault hash")
+@click.option("--token", "-t", default=DEFAULT_TOKEN, help="Personal access key for vault")
+@click.option("--vault", "-v", default=DEFAULT_PROJECT_ID, help="Vault ID")
 @click.argument("version_address", required=False)
 @click.pass_context
 def download(
         ctx: Context,
         version_address: str | None,
         directory: str, url: str | None, token: str | None, vault: str | None
 ) -> None:  # type: ignore
@@ -156,32 +161,36 @@
     client: KaasClient = ctx.obj["client"]
     vaults = client.list_vaults()
 
     if not vaults:
         click.echo("No vaults")
         return
 
-    for vault in vaults:
-        click.echo(vault)
+    vaults = [from_dict(data_class=Vault, data=item, config=Config(cast=[Vault])) for item in vaults]
+
+    filtered_data = [asdict(vault) for vault in vaults]
+    formatted_json = json.dumps(filtered_data, indent=4)
+    click.echo(f"Vaults:\n{formatted_json}")
 
 
 @cli.command(cls=CustomHelpOption, name="list-keys", help="List remote keys owned by <VAULT_ADDRESS>")
 @click.argument("vault_address", required=True)
 @click.pass_context
 def list_keys(ctx: Context, vault_address: str) -> None:
     client: KaasClient = ctx.obj["client"]
     keys = client.list_keys(vault_address)
 
     if not keys:
         click.echo(f"No keys found for vault {vault_address}")
         return
 
-    click.echo(f"Keys for vault {vault_address}:")
-    for key in keys:
-        click.echo(key)
+    keys = [from_dict(data_class=Key, data=item, config=Config(cast=[Key])) for item in keys]
+    filtered_data = [asdict(key) for key in keys]
+    formatted_json = json.dumps(filtered_data, indent=4)
+    click.echo(f"Keys for vault {vault_address}:\n{formatted_json}")
 
 
 @cli.command(cls=CustomHelpOption, name="list-versions",
              help="List remote versions of a cached artifact, with <VAULT_ADDRESS> as the address of the vault.")
 @click.argument("vault_address", required=True)
 @click.pass_context
 def list_versions(ctx: Context, vault_address: str) -> None:
@@ -189,16 +198,16 @@
     versions = client.list_versions(vault_address)
 
     if not versions:
         click.echo(f"No versions found for vault {vault_address}")
         return
 
     click.echo(f"Versions for vault {vault_address}:")
-    for version in versions:
-        click.echo(version)
+    formatted_json = json.dumps(versions, indent=4)
+    click.echo(formatted_json)
 
 
 @cli.command(cls=CustomHelpOption, name="logout", help="Log out from the system.")
 @click.pass_context
 def logout(ctx: Context) -> None:
     client: KaasClient = ctx.obj["client"]
     logout_success = client.logout()
```

### Comparing `kaas_cli-0.1.5/src/kaas_cli/client.py` & `kaas_cli-0.1.6/src/kaas_cli/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -196,15 +196,15 @@
         return json_data
 
     def _get_default_vault(self) -> str | None:
         try:
             json_data = self._session.get(url=f'{self._url}{USER_URL}')
         except Exception:
             raise KaasCliException("Get default vault failed") from None
-        vault_hash = jmespath.search('vaults[0].hash', json_data)
+        vault_hash = jmespath.search('vaults[0].id', json_data)
         return vault_hash
 
     def _get_upload_urls(self, metadata: dict[str, Any], vault: str) -> dict[str, Any]:
         data = self._session.post(
             url=f'{self._url}{FILES_URL.format(vault)}',
             data=json.dumps(metadata),
             headers={
@@ -341,23 +341,24 @@
         file_list = self._list_local_files(directory)
         if not file_list or len(file_list) == 0:
             raise ValueError(f'No files to upload in dir: {directory}')
 
         archive_name = self.get_version_from_digest(file_list)
         archive_path = self.archive_files(file_list, archive_name, archive_format='zip', root_dir=Path(directory))
         metadata = self.get_archive_metadata(archive_path)
-        print(f"Uploading {metadata} to S3...")
+
         vault: str | None = self._vault or self._get_default_vault()
         if vault is None:
             return UPLOAD_FAILURE_MESSAGE
         urls = self._get_upload_urls(metadata=metadata, vault=vault)
 
         try:
+            click.echo(f"Uploading {metadata} to S3...")
             self._upload_presigned_url(urls)
-            print(UPLOAD_SUCCESS_MESSAGE)
+            click.echo(UPLOAD_SUCCESS_MESSAGE)
         except Exception as e:
             raise KaasCliException(f"Failed to upload {archive_path} to S3: {e}") from None
         # remove the archive file after uploading
         os.remove(archive_path)
 
     def process_archive(self, archive_path: str, extract_to: str) -> None:
         """
@@ -587,18 +588,17 @@
         except Exception:
             raise KaasCliException("List vaults failed") from None
         return data
 
     def list_versions(self, vault: str) -> list[str]:
         try:
             data = self._get_download_url(vault)
-            print(data)
         except Exception:
             raise KaasCliException("List vaults failed") from None
-        return data
+        return data['data']
 
     def logout(self) -> bool:
         """
         Log out the user by clearing the session and authentication token.
         Returns True if the logout was successful, False otherwise.
         """
         try:
```

### Comparing `kaas_cli-0.1.5/src/kaas_cli/config.py` & `kaas_cli-0.1.6/src/kaas_cli/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 # Load environment variables from .flaskenv file
 load_dotenv('.flaskenv')
 
 DEFAULT_DIRECTORY = os.getenv('DEFAULT_DIRECTORY') or DEFAULT_K_OUT_FOLDER
 SERVER_URL = os.getenv('SERVER_URL') or DEFAULT_PROD_SERVER_URL
 DEFAULT_PROJECT_ID = os.getenv('DEFAULT_PROJECT_ID')
-DEFAULT_TOKEN = os.getenv('DEFAULT_TOKEN')
+DEFAULT_TOKEN = os.getenv('DEFAULT_KEY')
 
 
 class CustomHelpOption(click.Command):
     def __init__(self, *args: Any, **kwargs: Any) -> None:
         self.aliases = kwargs.pop('aliases', [])
         super().__init__(*args, **kwargs)
```

### Comparing `kaas_cli-0.1.5/src/kaas_cli/constants.py` & `kaas_cli-0.1.6/src/kaas_cli/constants.py`

 * *Files identical despite different names*

### Comparing `kaas_cli-0.1.5/PKG-INFO` & `kaas_cli-0.1.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: kaas-cli
-Version: 0.1.5
+Version: 0.1.6
 Summary: Command line utility for K as a Service
 Author: Runtime Verification, Inc.
 Author-email: contact@runtimeverification.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: click (>=8.0.1,<9.0.0)
+Requires-Dist: dacite (>=1.8.1,<2.0.0)
 Requires-Dist: gql[requests] (>=3.4.0,<4.0.0)
 Requires-Dist: hurry-filesize (>=0.9,<0.10)
 Requires-Dist: jmespath (>=1.0.1,<2.0.0)
 Requires-Dist: pytest (>=8.0.1,<9.0.0)
 Requires-Dist: pytest-watch (>=4.2.0,<5.0.0)
 Requires-Dist: python-dotenv (>=1.0.1,<2.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
@@ -25,15 +26,15 @@
 
 ## For Developers
 
 Prerequisites: `python >= 3.10`, `pip >= 20.0.2`, `poetry >= 1.3.2`.
 
 ### Installation
 
-To install the package using `pip`, start by building it:
+To install the package using `pip`, start by building from [Source](https://github.com/runtimeverification/kaas)
 
 ```bash
 make build
 pip install dist/*.whl
 ```
 
 Configure the CLI by copying the example environment file and setting up the necessary environment variables:
@@ -46,24 +47,25 @@
 
 ### Environment Variables
 
 Here's an overview of the environment variables:
 
 - **SERVER_URL**: The KaaS server API address for the main interaction within the CLI tool. This is a required field. For local development, use `http://localhost:5000`.
 - **DEFAULT_DIRECTORY**: The folder path for artifacts. This is an optional field. You can leave it empty.
-- **DEFAULT_PROJECT_ID**: Artifacts should be associated with a project ID. This is an optional field. You can leave it empty.
-- **DEFAULT_TOKEN**: If the user is not the owner of the project, they are required to provide a security token. This is an optional field. You can leave it empty.
+- **DEFAULT_VAULT_ID**: Artifacts should be associated with a project ID. This is an optional field. You can leave it empty.
+- **DEFAULT_KEY**: If the user is not the owner of the project, they are required to provide a security key. This is an optional field. You can leave it empty.
 
 ### Usage
 
 After installing the dependencies with `poetry install`, you can spawn a shell using `poetry shell`, or alternatively, use `make`:
 
 ```bash
 make shell
 kaas-cli hello
+kaas-cli --version
 ```
 
 To verify the installation, run `kaas-cli hello`. If you see the message `Hello World!`, the CLI is set up correctly.
 
 ### Documentation
 
 For detailed usage instructions of the `kaas-cli` tool, please refer to the official [documentation](https://docs.runtimeverification.com/kaas/guides/getting-started).
```

