# Comparing `tmp/langchain_cli-0.0.8.tar.gz` & `tmp/langchain_cli-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain_cli-0.0.8.tar", max compression
+gzip compressed data, was "langchain_cli-0.0.9.tar", max compression
```

## Comparing `langchain_cli-0.0.8.tar` & `langchain_cli-0.0.9.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0       96 2023-10-27 21:26:49.802216 langchain_cli-0.0.8/README.md
--rw-r--r--   0        0        0        0 2023-10-25 18:23:15.127847 langchain_cli-0.0.8/langchain_cli/__init__.py
--rw-r--r--   0        0        0      877 2023-10-27 21:26:45.224724 langchain_cli-0.0.8/langchain_cli/cli.py
--rw-r--r--   0        0        0      173 2023-10-26 20:30:47.220236 langchain_cli-0.0.8/langchain_cli/constants.py
--rw-r--r--   0        0        0      399 2023-10-27 13:34:05.829161 langchain_cli-0.0.8/langchain_cli/dev_scripts.py
--rw-r--r--   0        0        0        0 2023-10-25 18:23:15.128116 langchain_cli-0.0.8/langchain_cli/namespaces/__init__.py
--rw-r--r--   0        0        0     2942 2023-10-27 21:26:49.802329 langchain_cli-0.0.8/langchain_cli/namespaces/hub.py
--rw-r--r--   0        0        0     9055 2023-10-28 15:26:01.615684 langchain_cli-0.0.8/langchain_cli/namespaces/serve.py
--rw-r--r--   0        0        0     1072 2023-10-26 20:30:47.220783 langchain_cli-0.0.8/langchain_cli/package_template/LICENSE
--rw-r--r--   0        0        0       24 2023-10-26 20:30:47.220845 langchain_cli-0.0.8/langchain_cli/package_template/README.md
--rw-r--r--   0        0        0        0 2023-10-26 20:30:47.220939 langchain_cli-0.0.8/langchain_cli/package_template/package_template/__init__.py
--rw-r--r--   0        0        0      446 2023-10-27 13:34:05.830158 langchain_cli-0.0.8/langchain_cli/package_template/package_template/chain.py
--rw-r--r--   0        0        0      486 2023-10-27 21:26:45.224988 langchain_cli-0.0.8/langchain_cli/package_template/pyproject.toml
--rw-r--r--   0        0        0        0 2023-10-26 20:30:47.221160 langchain_cli-0.0.8/langchain_cli/package_template/tests/__init__.py
--rw-r--r--   0        0        0      832 2023-10-27 19:23:14.737842 langchain_cli-0.0.8/langchain_cli/project_template/README.md
--rw-r--r--   0        0        0        0 2023-10-26 20:30:47.221313 langchain_cli-0.0.8/langchain_cli/project_template/app/__init__.py
--rw-r--r--   0        0        0      252 2023-10-27 21:26:45.225076 langchain_cli-0.0.8/langchain_cli/project_template/app/server.py
--rw-r--r--   0        0        0        0 2023-10-26 20:30:47.221676 langchain_cli-0.0.8/langchain_cli/project_template/packages/README.md
--rw-r--r--   0        0        0      460 2023-10-27 21:26:45.225167 langchain_cli-0.0.8/langchain_cli/project_template/pyproject.toml
--rw-r--r--   0        0        0        0 2023-10-25 18:23:15.128600 langchain_cli-0.0.8/langchain_cli/utils/__init__.py
--rw-r--r--   0        0        0     1260 2023-10-27 13:34:05.830255 langchain_cli-0.0.8/langchain_cli/utils/events.py
--rw-r--r--   0        0        0     5885 2023-10-28 15:26:01.616306 langchain_cli-0.0.8/langchain_cli/utils/git.py
--rw-r--r--   0        0        0      585 2023-10-27 13:34:05.830476 langchain_cli-0.0.8/langchain_cli/utils/packages.py
--rw-r--r--   0        0        0     1122 2023-10-28 15:26:01.616540 langchain_cli-0.0.8/pyproject.toml
--rw-r--r--   0        0        0      816 1970-01-01 00:00:00.000000 langchain_cli-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0       96 2023-10-27 21:26:49.802216 langchain_cli-0.0.9/README.md
+-rw-r--r--   0        0        0        0 2023-10-25 18:23:15.127847 langchain_cli-0.0.9/langchain_cli/__init__.py
+-rw-r--r--   0        0        0     1031 2023-10-31 00:14:37.342584 langchain_cli-0.0.9/langchain_cli/cli.py
+-rw-r--r--   0        0        0      173 2023-10-26 20:30:47.220236 langchain_cli-0.0.9/langchain_cli/constants.py
+-rw-r--r--   0        0        0      401 2023-10-31 00:14:37.343916 langchain_cli-0.0.9/langchain_cli/dev_scripts.py
+-rw-r--r--   0        0        0        0 2023-10-25 18:23:15.128116 langchain_cli-0.0.9/langchain_cli/namespaces/__init__.py
+-rw-r--r--   0        0        0     7376 2023-10-31 00:14:37.344114 langchain_cli-0.0.9/langchain_cli/namespaces/app.py
+-rw-r--r--   0        0        0     3267 2023-10-31 00:14:37.344179 langchain_cli-0.0.9/langchain_cli/namespaces/template.py
+-rw-r--r--   0        0        0     1072 2023-10-26 20:30:47.220783 langchain_cli-0.0.9/langchain_cli/package_template/LICENSE
+-rw-r--r--   0        0        0     1692 2023-10-31 00:14:37.344790 langchain_cli-0.0.9/langchain_cli/package_template/README.md
+-rw-r--r--   0        0        0       45 2023-10-31 00:14:37.344872 langchain_cli-0.0.9/langchain_cli/package_template/package_template/__init__.py
+-rw-r--r--   0        0        0      446 2023-10-27 13:34:05.830158 langchain_cli-0.0.9/langchain_cli/package_template/package_template/chain.py
+-rw-r--r--   0        0        0      479 2023-10-31 00:14:37.345051 langchain_cli-0.0.9/langchain_cli/package_template/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-10-26 20:30:47.221160 langchain_cli-0.0.9/langchain_cli/package_template/tests/__init__.py
+-rw-r--r--   0        0        0     1192 2023-10-31 00:14:37.345142 langchain_cli-0.0.9/langchain_cli/project_template/README.md
+-rw-r--r--   0        0        0        0 2023-10-26 20:30:47.221313 langchain_cli-0.0.9/langchain_cli/project_template/app/__init__.py
+-rw-r--r--   0        0        0      252 2023-10-27 21:26:45.225076 langchain_cli-0.0.9/langchain_cli/project_template/app/server.py
+-rw-r--r--   0        0        0        0 2023-10-26 20:30:47.221676 langchain_cli-0.0.9/langchain_cli/project_template/packages/README.md
+-rw-r--r--   0        0        0      460 2023-10-29 05:16:15.283742 langchain_cli-0.0.9/langchain_cli/project_template/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-10-25 18:23:15.128600 langchain_cli-0.0.9/langchain_cli/utils/__init__.py
+-rw-r--r--   0        0        0     1260 2023-10-27 13:34:05.830255 langchain_cli-0.0.9/langchain_cli/utils/events.py
+-rw-r--r--   0        0        0     6297 2023-10-31 00:14:37.345817 langchain_cli-0.0.9/langchain_cli/utils/git.py
+-rw-r--r--   0        0        0      585 2023-10-27 13:34:05.830476 langchain_cli-0.0.9/langchain_cli/utils/packages.py
+-rw-r--r--   0        0        0     1122 2023-10-31 00:16:01.151049 langchain_cli-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0      816 1970-01-01 00:00:00.000000 langchain_cli-0.0.9/PKG-INFO
```

### Comparing `langchain_cli-0.0.8/langchain_cli/namespaces/hub.py` & `langchain_cli-0.0.9/langchain_cli/namespaces/template.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,91 +1,102 @@
 """
-Manage installable hub packages.
+Develop installable templates.
 """
 
 import re
 import shutil
 import subprocess
 from pathlib import Path
 from typing import Optional
 
 import typer
 from langserve.packages import get_langserve_export
 from typing_extensions import Annotated
 
 from langchain_cli.utils.packages import get_package_root
 
-hub = typer.Typer(no_args_is_help=True, add_completion=False)
+package_cli = typer.Typer(no_args_is_help=True, add_completion=False)
 
 
-@hub.command()
+@package_cli.command()
 def new(
     name: Annotated[str, typer.Argument(help="The name of the folder to create")],
     with_poetry: Annotated[
         bool,
         typer.Option("--with-poetry/--no-poetry", help="Don't run poetry install"),
     ] = False,
 ):
     """
-    Creates a new hub package.
+    Creates a new template package.
     """
     computed_name = name if name != "." else Path.cwd().name
     destination_dir = Path.cwd() / name if name != "." else Path.cwd()
 
     # copy over template from ../package_template
     project_template_dir = Path(__file__).parents[1] / "package_template"
     shutil.copytree(project_template_dir, destination_dir, dirs_exist_ok=name == ".")
 
     package_name_split = computed_name.split("/")
-    package_name_last = (
+    package_name = (
         package_name_split[-2]
         if len(package_name_split) > 1 and package_name_split[-1] == ""
         else package_name_split[-1]
     )
-    default_package_name = re.sub(
+    module_name = re.sub(
         r"[^a-zA-Z0-9_]",
         "_",
-        package_name_last,
+        package_name,
+    )
+
+    # generate app route code
+    chain_name = f"{module_name}_chain"
+    app_route_code = (
+        f"from {module_name} import chain as {chain_name}\n\n"
+        f'add_routes(app, {chain_name}, path="/{package_name}")'
     )
 
     # replace template strings
     pyproject = destination_dir / "pyproject.toml"
     pyproject_contents = pyproject.read_text()
     pyproject.write_text(
-        pyproject_contents.replace("__package_name__", default_package_name)
+        pyproject_contents.replace("__package_name__", module_name).replace(
+            "__module_name__", module_name
+        )
     )
 
     # move module folder
-    package_dir = destination_dir / default_package_name
+    package_dir = destination_dir / module_name
     shutil.move(destination_dir / "package_template", package_dir)
 
     # replace readme
     readme = destination_dir / "README.md"
     readme_contents = readme.read_text()
     readme.write_text(
-        readme_contents.replace("__package_name_last__", package_name_last)
+        readme_contents.replace("__package_name_last__", package_name).replace(
+            "__app_route_code__", app_route_code
+        )
     )
 
     # poetry install
     if with_poetry:
         subprocess.run(["poetry", "install"], cwd=destination_dir)
 
 
-@hub.command()
-def start(
+@package_cli.command()
+def serve(
     *,
     port: Annotated[
         Optional[int], typer.Option(help="The port to run the server on")
     ] = None,
     host: Annotated[
         Optional[str], typer.Option(help="The host to run the server on")
     ] = None,
 ) -> None:
     """
-    Starts a demo LangServe instance for this hub package.
+    Starts a demo app for this template.
     """
     # load pyproject.toml
     project_dir = get_package_root()
     pyproject = project_dir / "pyproject.toml"
 
     # get langserve export - throws KeyError if invalid
     get_langserve_export(pyproject)
```

### Comparing `langchain_cli-0.0.8/langchain_cli/namespaces/serve.py` & `langchain_cli-0.0.9/langchain_cli/namespaces/app.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,105 +1,85 @@
 """
-Manage LangServe application projects.
+Manage LangChain apps
 """
 
 import shutil
 import subprocess
 from pathlib import Path
 from typing import Dict, List, Optional, Tuple
 
 import typer
-from langserve.packages import get_langserve_export, list_packages
+from langserve.packages import get_langserve_export
 from typing_extensions import Annotated
 
 from langchain_cli.utils.events import create_events
 from langchain_cli.utils.git import (
     DependencySource,
     copy_repo,
     parse_dependencies,
     update_repo,
 )
 from langchain_cli.utils.packages import get_package_root
 
 REPO_DIR = Path(typer.get_app_dir("langchain")) / "git_repos"
 
-serve = typer.Typer(no_args_is_help=True, add_completion=False)
+app_cli = typer.Typer(no_args_is_help=True, add_completion=False)
 
 
-@serve.command()
+@app_cli.command()
 def new(
     name: Annotated[str, typer.Argument(help="The name of the folder to create")],
     *,
     package: Annotated[
         Optional[List[str]],
         typer.Option(help="Packages to seed the project with"),
     ] = None,
-    with_poetry: Annotated[
-        bool,
-        typer.Option("--with-poetry/--no-poetry", help="Run poetry install"),
-    ] = False,
 ):
     """
     Create a new LangServe application.
     """
     # copy over template from ../project_template
     project_template_dir = Path(__file__).parents[1] / "project_template"
     destination_dir = Path.cwd() / name if name != "." else Path.cwd()
+    app_name = name if name != "." else Path.cwd().name
     shutil.copytree(project_template_dir, destination_dir, dirs_exist_ok=name == ".")
 
-    # poetry install
-    if with_poetry:
-        subprocess.run(["poetry", "install"], cwd=destination_dir)
+    readme = destination_dir / "README.md"
+    readme_contents = readme.read_text()
+    readme.write_text(readme_contents.replace("__app_name__", app_name))
 
     # add packages if specified
     if package is not None and len(package) > 0:
-        add(package, project_dir=destination_dir, with_poetry=with_poetry)
+        add(package, project_dir=destination_dir)
 
 
-@serve.command()
-def install():
-    package_root = get_package_root() / "packages"
-    for package_path in list_packages(package_root):
-        try:
-            pyproject_path = package_path / "pyproject.toml"
-            langserve_export = get_langserve_export(pyproject_path)
-            typer.echo(f"Installing {langserve_export['package_name']}...")
-            subprocess.run(["poetry", "add", "--editable", package_path])
-        except Exception as e:
-            typer.echo(f"Skipping installing {package_path} due to error: {e}")
-
-
-@serve.command()
+@app_cli.command()
 def add(
     dependencies: Annotated[
         Optional[List[str]], typer.Argument(help="The dependency to add")
     ] = None,
     *,
     api_path: Annotated[List[str], typer.Option(help="API paths to add")] = [],
     project_dir: Annotated[
         Optional[Path], typer.Option(help="The project directory")
     ] = None,
     repo: Annotated[
-        List[str], typer.Option(help="Install deps from a specific github repo instead")
+        List[str],
+        typer.Option(help="Install templates from a specific github repo instead"),
     ] = [],
     branch: Annotated[
-        List[str], typer.Option(help="Install deps from a specific branch")
+        List[str], typer.Option(help="Install templates from a specific branch")
     ] = [],
-    with_poetry: Annotated[
-        bool,
-        typer.Option("--with-poetry/--no-poetry", help="Run poetry install"),
-    ] = False,
 ):
     """
-    Adds the specified package to the current LangServe instance.
+    Adds the specified template to the current LangServe app.
 
     e.g.:
-    langchain serve add extraction-openai-functions
-    langchain serve add git+ssh://git@github.com/efriis/simple-pirate.git
-    langchain serve add git+https://github.com/efriis/hub.git#devbranch#subdirectory=mypackage
+    langchain app add extraction-openai-functions
+    langchain app add git+ssh://git@github.com/efriis/simple-pirate.git
     """
 
     parsed_deps = parse_dependencies(dependencies, repo, branch, api_path)
 
     project_root = get_package_root(project_dir)
 
     package_dir = project_root / "packages"
@@ -119,15 +99,15 @@
     installed_destination_paths: List[Path] = []
     installed_exports: List[Dict] = []
 
     for (git, ref), group_deps in grouped.items():
         if len(group_deps) == 1:
             typer.echo(f"Adding {git}@{ref}...")
         else:
-            typer.echo(f"Adding {len(group_deps)} dependencies from {git}@{ref}")
+            typer.echo(f"Adding {len(group_deps)} templates from {git}@{ref}")
         source_repo_path = update_repo(git, ref, REPO_DIR)
 
         for dep in group_deps:
             source_path = (
                 source_repo_path / dep["subdirectory"]
                 if dep["subdirectory"]
                 else source_repo_path
@@ -156,28 +136,22 @@
         typer.echo("No packages installed. Exiting.")
         return
 
     cwd = Path.cwd()
     installed_desination_strs = [
         str(p.relative_to(cwd)) for p in installed_destination_paths
     ]
+    cmd = ["pip", "install", "-e"] + installed_desination_strs
+    cmd_str = " \\\n  ".join(installed_desination_strs)
+    install_str = f"To install:\n\npip install -e \\\n  {cmd_str}"
+    typer.echo(install_str)
 
-    if with_poetry:
-        subprocess.run(
-            ["poetry", "add", "--editable"] + installed_desination_strs,
-            cwd=cwd,
-        )
-    else:
-        cmd = ["pip", "install", "-e"] + installed_desination_strs
-        cmd_str = " \\\n  ".join(installed_desination_strs)
-        install_str = f"To install:\n\npip install -e \\\n  {cmd_str}"
-        typer.echo(install_str)
+    if typer.confirm("Run it?"):
+        subprocess.run(cmd, cwd=cwd)
 
-        if typer.confirm("Run it?"):
-            subprocess.run(cmd, cwd=cwd)
     if typer.confirm("\nGenerate route code for these packages?", default=True):
         chain_names = []
         for e in installed_exports:
             original_candidate = f'{e["package_name"].replace("-", "_")}_chain'
             candidate = original_candidate
             i = 2
             while candidate in chain_names:
@@ -196,71 +170,57 @@
         ]
         routes = [
             f'add_routes(app, {name}, path="{path}")'
             for name, path in zip(chain_names, api_paths)
         ]
 
         lines = (
-            ["", "Great! Add the following to your app:", ""] + imports + [""] + routes
+            ["", "Great! Add the following to your app:\n\n```", ""]
+            + imports
+            + [""]
+            + routes
+            + ["```"]
         )
         typer.echo("\n".join(lines))
 
 
-@serve.command()
+@app_cli.command()
 def remove(
     api_paths: Annotated[List[str], typer.Argument(help="The API paths to remove")],
-    with_poetry: Annotated[
-        bool,
-        typer.Option("--with_poetry/--no-poetry", help="Don't run poetry remove"),
-    ] = False,
 ):
     """
-    Removes the specified package from the current LangServe instance.
+    Removes the specified package from the current LangServe app.
     """
     for api_path in api_paths:
         package_dir = Path.cwd() / "packages" / api_path
         if not package_dir.exists():
             typer.echo(f"Endpoint {api_path} does not exist. Skipping...")
             continue
         pyproject = package_dir / "pyproject.toml"
         langserve_export = get_langserve_export(pyproject)
         typer.echo(f"Removing {langserve_export['package_name']}...")
-        if with_poetry:
-            subprocess.run(["poetry", "remove", langserve_export["package_name"]])
-        shutil.rmtree(package_dir)
-
 
-@serve.command()
-def list():
-    """
-    Lists all packages in the current LangServe instance.
-    """
-    package_root = get_package_root() / "packages"
-    for package_path in list_packages(package_root):
-        relative = package_path.relative_to(package_root)
-        pyproject_path = package_path / "pyproject.toml"
-        langserve_export = get_langserve_export(pyproject_path)
-        typer.echo(
-            f"{relative}: ({langserve_export['module']}.{langserve_export['attr']})"
-        )
+        shutil.rmtree(package_dir)
 
 
-@serve.command()
-def start(
+@app_cli.command()
+def serve(
     *,
     port: Annotated[
         Optional[int], typer.Option(help="The port to run the server on")
     ] = None,
     host: Annotated[
         Optional[str], typer.Option(help="The host to run the server on")
     ] = None,
-    app: Annotated[Optional[str], typer.Option(help="The app to run")] = None,
+    app: Annotated[
+        Optional[str], typer.Option(help="The app to run, e.g. `app.server:app`")
+    ] = None,
 ) -> None:
     """
-    Starts the LangServe instance.
+    Starts the LangServe app.
     """
 
     app_str = app if app is not None else "app.server:app"
     port_str = str(port) if port is not None else "8000"
     host_str = host if host is not None else "127.0.0.1"
 
     cmd = ["uvicorn", app_str, "--reload", "--port", port_str, "--host", host_str]
```

### Comparing `langchain_cli-0.0.8/langchain_cli/package_template/LICENSE` & `langchain_cli-0.0.9/langchain_cli/package_template/LICENSE`

 * *Files identical despite different names*

### Comparing `langchain_cli-0.0.8/langchain_cli/utils/events.py` & `langchain_cli-0.0.9/langchain_cli/utils/events.py`

 * *Files identical despite different names*

### Comparing `langchain_cli-0.0.8/langchain_cli/utils/git.py` & `langchain_cli-0.0.9/langchain_cli/utils/git.py`

 * *Files 18% similar despite different names*

```diff
@@ -128,50 +128,60 @@
         (dependencies and len(dependencies) != num_deps)
         or (api_path and len(api_path) != num_deps)
         or (repo and len(repo) not in [1, num_deps])
         or (branch and len(branch) not in [1, num_deps])
     ):
         raise ValueError(
             "Number of defined repos/branches/api_paths did not match the "
-            "number of dependencies."
+            "number of templates."
         )
     inner_deps = _list_arg_to_length(dependencies, num_deps)
     inner_api_paths = _list_arg_to_length(api_path, num_deps)
     inner_repos = _list_arg_to_length(repo, num_deps)
     inner_branches = _list_arg_to_length(branch, num_deps)
 
     return [
         parse_dependency_string(iter_dep, iter_repo, iter_branch, iter_api_path)
         for iter_dep, iter_repo, iter_branch, iter_api_path in zip(
             inner_deps, inner_repos, inner_branches, inner_api_paths
         )
     ]
 
 
-def _get_repo_path(gitstring: str, repo_dir: Path) -> Path:
+def _get_repo_path(gitstring: str, ref: Optional[str], repo_dir: Path) -> Path:
     # only based on git for now
-    hashed = hashlib.sha256(gitstring.encode("utf-8")).hexdigest()[:8]
+    ref_str = ref if ref is not None else ""
+    hashed = hashlib.sha256((f"{gitstring}:{ref_str}").encode("utf-8")).hexdigest()[:8]
 
     removed_protocol = gitstring.split("://")[-1]
     removed_basename = re.split(r"[/:]", removed_protocol, 1)[-1]
     removed_extras = removed_basename.split("#")[0]
     foldername = re.sub(r"[^a-zA-Z0-9_]", "_", removed_extras)
 
     directory_name = f"{foldername}_{hashed}"
     return repo_dir / directory_name
 
 
 def update_repo(gitstring: str, ref: Optional[str], repo_dir: Path) -> Path:
     # see if path already saved
-    repo_path = _get_repo_path(gitstring, repo_dir)
+    repo_path = _get_repo_path(gitstring, ref, repo_dir)
     if repo_path.exists():
-        shutil.rmtree(repo_path)
+        # try pulling
+        try:
+            repo = Repo(repo_path)
+            if repo.active_branch.name != ref:
+                raise ValueError()
+            repo.remotes.origin.pull()
+        except Exception:
+            # if it fails, delete and clone again
+            shutil.rmtree(repo_path)
+            Repo.clone_from(gitstring, repo_path, branch=ref, depth=1)
+    else:
+        Repo.clone_from(gitstring, repo_path, branch=ref, depth=1)
 
-    # now we have fresh dir
-    Repo.clone_from(gitstring, repo_path, branch=ref, depth=1)
     return repo_path
 
 
 def copy_repo(
     source: Path,
     destination: Path,
 ) -> None:
```

### Comparing `langchain_cli-0.0.8/langchain_cli/utils/packages.py` & `langchain_cli-0.0.9/langchain_cli/utils/packages.py`

 * *Files identical despite different names*

### Comparing `langchain_cli-0.0.8/pyproject.toml` & `langchain_cli-0.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "langchain-cli"
-version = "0.0.8"
+version = "0.0.9"
 description = "CLI for interacting with LangChain"
 authors = ["Erick Friis <erick@langchain.dev>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 typer = {extras = ["all"], version = "^0.9.0"}
```

### Comparing `langchain_cli-0.0.8/PKG-INFO` & `langchain_cli-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langchain-cli
-Version: 0.0.8
+Version: 0.0.9
 Summary: CLI for interacting with LangChain
 Author: Erick Friis
 Author-email: erick@langchain.dev
 Requires-Python: >=3.8.1,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

