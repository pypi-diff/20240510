# Comparing `tmp/mdremotifier-0.3.1.tar.gz` & `tmp/mdremotifier-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/mnt/c/gdrive/code/markdown-remotifier/dist/.tmp-0ti6hz2y/mdremotifier-0.3.1.tar", last modified: Sat May  4 21:17:42 2024, max compression
+gzip compressed data, was "/mnt/c/gdrive/code/markdown-remotifier/dist/.tmp-eqw7j0uo/mdremotifier-0.3.2.tar", last modified: Fri May 10 07:06:56 2024, max compression
```

## Comparing `mdremotifier-0.3.1.tar` & `mdremotifier-0.3.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0 realz     (1000) realz     (1000)        0 2024-05-04 21:17:42.096151 mdremotifier-0.3.1/
-drwxrwxrwx   0 realz     (1000) realz     (1000)        0 2024-05-04 21:17:41.943652 mdremotifier-0.3.1/.github/
--rwxrwxrwx   0 realz     (1000) realz     (1000)    15622 2024-05-04 21:09:57.000000 mdremotifier-0.3.1/.github/README.remotified.md
--rwxrwxrwx   0 realz     (1000) realz     (1000)     1102 2024-04-27 14:17:24.000000 mdremotifier-0.3.1/LICENSE.md
--rwxrwxrwx   0 realz     (1000) realz     (1000)    22411 2024-05-04 21:17:42.089640 mdremotifier-0.3.1/PKG-INFO
--rwxrwxrwx   0 realz     (1000) realz     (1000)    14493 2024-05-04 21:09:57.000000 mdremotifier-0.3.1/README.md
-drwxrwxrwx   0 realz     (1000) realz     (1000)        0 2024-05-04 21:17:41.970792 mdremotifier-0.3.1/mdremotifier/
--rwxrwxrwx   0 realz     (1000) realz     (1000)      396 2024-04-27 10:02:01.000000 mdremotifier-0.3.1/mdremotifier/__init__.py
--rwxrwxrwx   0 realz     (1000) realz     (1000)     9627 2024-05-04 21:09:57.000000 mdremotifier-0.3.1/mdremotifier/cli.py
-drwxrwxrwx   0 realz     (1000) realz     (1000)        0 2024-05-04 21:17:42.070554 mdremotifier-0.3.1/mdremotifier.egg-info/
--rwxrwxrwx   0 realz     (1000) realz     (1000)    22411 2024-05-04 21:17:41.000000 mdremotifier-0.3.1/mdremotifier.egg-info/PKG-INFO
--rwxrwxrwx   0 realz     (1000) realz     (1000)      327 2024-05-04 21:17:41.000000 mdremotifier-0.3.1/mdremotifier.egg-info/SOURCES.txt
--rwxrwxrwx   0 realz     (1000) realz     (1000)        1 2024-05-04 21:17:41.000000 mdremotifier-0.3.1/mdremotifier.egg-info/dependency_links.txt
--rwxrwxrwx   0 realz     (1000) realz     (1000)       55 2024-05-04 21:17:41.000000 mdremotifier-0.3.1/mdremotifier.egg-info/entry_points.txt
--rwxrwxrwx   0 realz     (1000) realz     (1000)     1848 2024-05-04 21:17:41.000000 mdremotifier-0.3.1/mdremotifier.egg-info/requires.txt
--rwxrwxrwx   0 realz     (1000) realz     (1000)       13 2024-05-04 21:17:41.000000 mdremotifier-0.3.1/mdremotifier.egg-info/top_level.txt
--rwxrwxrwx   0 realz     (1000) realz     (1000)     4075 2024-05-04 21:09:57.000000 mdremotifier-0.3.1/pyproject.toml
--rwxrwxrwx   0 realz     (1000) realz     (1000)       38 2024-05-04 21:17:42.096151 mdremotifier-0.3.1/setup.cfg
+drwxrwxrwx   0 realz     (1000) realz     (1000)        0 2024-05-10 07:06:56.439402 mdremotifier-0.3.2/
+drwxrwxrwx   0 realz     (1000) realz     (1000)        0 2024-05-10 07:06:56.067703 mdremotifier-0.3.2/.github/
+-rwxrwxrwx   0 realz     (1000) realz     (1000)    15714 2024-05-10 07:06:04.000000 mdremotifier-0.3.2/.github/README.remotified.md
+-rwxrwxrwx   0 realz     (1000) realz     (1000)     1102 2024-04-27 14:17:24.000000 mdremotifier-0.3.2/LICENSE.md
+-rwxrwxrwx   0 realz     (1000) realz     (1000)    22551 2024-05-10 07:06:56.424216 mdremotifier-0.3.2/PKG-INFO
+-rwxrwxrwx   0 realz     (1000) realz     (1000)    14585 2024-05-10 07:06:04.000000 mdremotifier-0.3.2/README.md
+drwxrwxrwx   0 realz     (1000) realz     (1000)        0 2024-05-10 07:06:56.133022 mdremotifier-0.3.2/mdremotifier/
+-rwxrwxrwx   0 realz     (1000) realz     (1000)      396 2024-04-27 10:02:01.000000 mdremotifier-0.3.2/mdremotifier/__init__.py
+-rwxrwxrwx   0 realz     (1000) realz     (1000)     9627 2024-05-04 21:09:57.000000 mdremotifier-0.3.2/mdremotifier/cli.py
+drwxrwxrwx   0 realz     (1000) realz     (1000)        0 2024-05-10 07:06:56.381365 mdremotifier-0.3.2/mdremotifier.egg-info/
+-rwxrwxrwx   0 realz     (1000) realz     (1000)    22551 2024-05-10 07:06:55.000000 mdremotifier-0.3.2/mdremotifier.egg-info/PKG-INFO
+-rwxrwxrwx   0 realz     (1000) realz     (1000)      327 2024-05-10 07:06:55.000000 mdremotifier-0.3.2/mdremotifier.egg-info/SOURCES.txt
+-rwxrwxrwx   0 realz     (1000) realz     (1000)        1 2024-05-10 07:06:55.000000 mdremotifier-0.3.2/mdremotifier.egg-info/dependency_links.txt
+-rwxrwxrwx   0 realz     (1000) realz     (1000)       55 2024-05-10 07:06:55.000000 mdremotifier-0.3.2/mdremotifier.egg-info/entry_points.txt
+-rwxrwxrwx   0 realz     (1000) realz     (1000)     1865 2024-05-10 07:06:55.000000 mdremotifier-0.3.2/mdremotifier.egg-info/requires.txt
+-rwxrwxrwx   0 realz     (1000) realz     (1000)       13 2024-05-10 07:06:55.000000 mdremotifier-0.3.2/mdremotifier.egg-info/top_level.txt
+-rwxrwxrwx   0 realz     (1000) realz     (1000)     4097 2024-05-10 07:06:04.000000 mdremotifier-0.3.2/pyproject.toml
+-rwxrwxrwx   0 realz     (1000) realz     (1000)       38 2024-05-10 07:06:56.440411 mdremotifier-0.3.2/setup.cfg
```

### Comparing `mdremotifier-0.3.1/.github/README.remotified.md` & `mdremotifier-0.3.2/.github/README.remotified.md`

 * *Files 4% similar despite different names*

```diff
@@ -62,64 +62,67 @@
 |                   | Status                      | Stable                    | Unstable                  |                    |
 | ----------------- | --------------------------- | ------------------------- | ------------------------- | ------------------ |
 | **[Master][10]**  | [![Build and Test][11]][12] | [![since tagged][13]][14] |                           | ![last commit][15] |
 | **[Develop][16]** | [![Build and Test][17]][12] | [![since tagged][18]][19] | [![since tagged][20]][21] | ![last commit][22] |
 
 </div>
 
-<img alt="Demo" src="https://raw.githubusercontent.com/realazthat/mdremotifier/v0.3.1/.github/demo.gif" width="100%"/>
+<img alt="Demo" src="https://raw.githubusercontent.com/realazthat/mdremotifier/v0.3.2/.github/demo.gif" width="100%"/>
 
 ## ❔ What
 
 What mdremotifier does:
 
-Turn this ([./mdremotifier/examples/EXAMPLE.md](https://github.com/realazthat/mdremotifier/blob/v0.3.1/mdremotifier/examples/EXAMPLE.md)):
+Turn this ([./mdremotifier/examples/EXAMPLE.md](https://github.com/realazthat/mdremotifier/blob/v0.3.2/mdremotifier/examples/EXAMPLE.md)):
 
 <!---->
 ```md
 # Example markdown file
 
 A link to a local file [LICENSE.md](./LICENSE.md).
 
 ```
 <!---->
 
 Into this
-([./mdremotifier/examples/EXAMPLE.remotified.md](https://github.com/realazthat/mdremotifier/blob/v0.3.1/mdremotifier/examples/EXAMPLE.remotified.md)):
+([./mdremotifier/examples/EXAMPLE.remotified.md](https://github.com/realazthat/mdremotifier/blob/v0.3.2/mdremotifier/examples/EXAMPLE.remotified.md)):
 
 <!---->
 ```md
 # Example markdown file
 
 A link to a local file [LICENSE.md](https://raw.githubusercontent.com/realazthat/mdremotifier/master/LICENSE.md).
 
 ```
 <!---->
 
 This is useful for uploading `README.md` files to third-party sites, like the
 npmjs.com registry, or pypi.org registry, because these registries will break
 the local images in your README when displayed on their sites.
 
+See <https://pypi.org/project/mdremotifier/>, notice how all of the images are
+not broken.
+
 ## 🎇 Features
 
 - 📷🔗📡🌐🖼️ Replace local URLs with raw.githubusercontent.com URLs.
 
 ## 🏠 Installation
 
 ```bash
 # Install from pypi (https://pypi.org/project/mdremotifier/)
 pip install mdremotifier
 
 # Install from git (https://github.com/realazthat/mdremotifier)
-pip install git+https://github.com/realazthat/mdremotifier.git@v0.3.1
+pip install git+https://github.com/realazthat/mdremotifier.git@v0.3.2
 ```
 
 ## 🚜 Usage
 
-Example README: ([./mdremotifier/examples/EXAMPLE.md](https://github.com/realazthat/mdremotifier/blob/v0.3.1/mdremotifier/examples/EXAMPLE.md)):
+Example README: ([./mdremotifier/examples/EXAMPLE.md](https://github.com/realazthat/mdremotifier/blob/v0.3.2/mdremotifier/examples/EXAMPLE.md)):
 
 <!---->
 ```md
 # Example markdown file
 
 A link to a local file [LICENSE.md](./LICENSE.md).
 
@@ -137,29 +140,29 @@
 
 ```
 <!---->
 
 ## 💻 Command Line Options
 
 <!---->
-<img alt="Output of `python -m mdremotifier.cli --help`" src="https://raw.githubusercontent.com/realazthat/mdremotifier/v0.3.1/README.help.generated.svg"/>
+<img alt="Output of `python -m mdremotifier.cli --help`" src="https://raw.githubusercontent.com/realazthat/mdremotifier/v0.3.2/README.help.generated.svg"/>
 <!-- -->
 
 ## 💡 Examples
 
 - mdremotifier's own `README`:
-  - Original: [./README.md](https://github.com/realazthat/mdremotifier/blob/v0.3.1/README.md).
-  - Remotified: [./.github/README.remotified.md](https://github.com/realazthat/mdremotifier/blob/v0.3.1/.github/README.remotified.md).
-  - Generation script: [./scripts/generate-readme.sh](https://github.com/realazthat/mdremotifier/blob/v0.3.1/scripts/generate-readme.sh).
+  - Original: [./README.md](https://github.com/realazthat/mdremotifier/blob/v0.3.2/README.md).
+  - Remotified: [./.github/README.remotified.md](https://github.com/realazthat/mdremotifier/blob/v0.3.2/.github/README.remotified.md).
+  - Generation script: [./scripts/generate-readme.sh](https://github.com/realazthat/mdremotifier/blob/v0.3.2/scripts/generate-readme.sh).
 - Example:
-  - Original: [./mdremotifier/examples/EXAMPLE.md](https://github.com/realazthat/mdremotifier/blob/v0.3.1/mdremotifier/examples/EXAMPLE.md).
+  - Original: [./mdremotifier/examples/EXAMPLE.md](https://github.com/realazthat/mdremotifier/blob/v0.3.2/mdremotifier/examples/EXAMPLE.md).
   - Remotified:
-    [./mdremotifier/examples/EXAMPLE.remotified.md](https://github.com/realazthat/mdremotifier/blob/v0.3.1/mdremotifier/examples/EXAMPLE.remotified.md).
+    [./mdremotifier/examples/EXAMPLE.remotified.md](https://github.com/realazthat/mdremotifier/blob/v0.3.2/mdremotifier/examples/EXAMPLE.remotified.md).
   - Generation script:
-    [./mdremotifier/examples/example.sh](https://github.com/realazthat/mdremotifier/blob/v0.3.1/mdremotifier/examples/example.sh).
+    [./mdremotifier/examples/example.sh](https://github.com/realazthat/mdremotifier/blob/v0.3.2/mdremotifier/examples/example.sh).
 
 <!-- TODO: Rebuild this for mdremotifier
 - Projects using mdremotifier:
   - [realazthat/snipinator](https://github.com/realazthat/snipinator), See
     [snipinator/README.md.jinja2](https://github.com/realazthat/snipinator/blob/61cb88593baa099dc375cf5fd40679e4be673fc5/README.md.jinja2).
   - [github.com/realazthat/changeguard](https://github.com/realazthat/changeguard),
     See
@@ -182,25 +185,25 @@
 - Python 3.8+
   - Why: Some dev dependencies require Python 3.8+.
 
 ### Tested Platforms
 
 - WSL2 Ubuntu 20.04, Python `3.8.0`.
 - Ubuntu 20.04, Python `3.8.0, 3.9.0, 3.10.0, 3.11.0, 3.12.0`, tested in GitHub Actions
-  workflow ([build-and-test.yml](https://github.com/realazthat/mdremotifier/blob/v0.3.1/.github/workflows/build-and-test.yml)).
+  workflow ([build-and-test.yml](https://github.com/realazthat/mdremotifier/blob/v0.3.2/.github/workflows/build-and-test.yml)).
 
 ## 🤏 Versioning
 
 We use SemVer for versioning. For the versions available, see the tags on this
 repository.
 
 ## 🔑 License
 
 This project is licensed under the MIT License - see the
-[./LICENSE.md](https://github.com/realazthat/mdremotifier/blob/v0.3.1/LICENSE.md) file for details.
+[./LICENSE.md](https://github.com/realazthat/mdremotifier/blob/v0.3.2/LICENSE.md) file for details.
 
 ## 🙏 Thanks
 
 Main libraries used in mdremotifier are:
 
 - Markdown AST: [mistletoe](https://github.com/miyuchina/mistletoe).
 - Colorful CLI help: [rich-argparse](https://github.com/hamdanal/rich-argparse).
@@ -224,15 +227,15 @@
 
 ## 🫡 Contributions
 
 ### Development environment: Linux-like
 
 - For running `pre.sh` (Linux-like environment).
 
-  - From [./.github/dependencies.yml](https://github.com/realazthat/mdremotifier/blob/v0.3.1/.github/dependencies.yml), which is used for
+  - From [./.github/dependencies.yml](https://github.com/realazthat/mdremotifier/blob/v0.3.2/.github/dependencies.yml), which is used for
     the GH Action to do a fresh install of everything:
 
     ```yaml
     bash: scripts.
     findutils: scripts.
     grep: tests.
     xxd: tests.
@@ -243,47 +246,47 @@
     jq: dependency for [yq](https://github.com/kislyuk/yq), which is used to generate
       the README; the README generator needs to use `tomlq` (which is a part of `yq`)
       to query `pyproject.toml`.
 
     ```
 
   - Requires `pyenv`, or an exact matching version of python as in
-    [.python-version](https://github.com/realazthat/mdremotifier/blob/v0.3.1/.python-version) (which is currently
+    [.python-version](https://github.com/realazthat/mdremotifier/blob/v0.3.2/.python-version) (which is currently
     `3.8.0 `).
   - `jq`, ([installation](https://jqlang.github.io/jq/)) required for
     [yq](https://github.com/kislyuk/yq), which is itself required for our
-    [./README.md](https://github.com/realazthat/mdremotifier/blob/v0.3.1/README.md) generation, which uses `tomlq` (from the
+    [./README.md](https://github.com/realazthat/mdremotifier/blob/v0.3.2/README.md) generation, which uses `tomlq` (from the
     [yq](https://github.com/kislyuk/yq) package) to include version strings from
-    [./pyproject.toml](https://github.com/realazthat/mdremotifier/blob/v0.3.1/pyproject.toml).
+    [./pyproject.toml](https://github.com/realazthat/mdremotifier/blob/v0.3.2/pyproject.toml).
   - act (to run the GH Action locally):
     - Requires nodejs.
     - Requires Go.
     - docker.
   - Generate animation:
     - docker
 
 ### Commit Process
 
 1. (Optionally) Fork the `develop` branch.
 2. Stage your files: `git add path/to/file.py`.
 3. `bash ./scripts/pre.sh`, this will format, lint, and test the code.
 4. `git status` check if anything changed (generated
-   [./README.md](https://github.com/realazthat/mdremotifier/blob/v0.3.1/README.md) for example), if so, `git add` the
+   [./README.md](https://github.com/realazthat/mdremotifier/blob/v0.3.2/README.md) for example), if so, `git add` the
    changes, and go back to the previous step.
 5. `git commit -m "..."`.
 6. Make a PR to `develop` (or push to develop if you have the rights).
 
 ## 🔄🚀 Release Process
 
 These instructions are for maintainers of the project.
 
 1. In the `develop` branch, run `bash ./scripts/pre.sh` to ensure
    everything is in order.
 2. In the `develop` branch, bump the version in
-   [./pyproject.toml](https://github.com/realazthat/mdremotifier/blob/v0.3.1/pyproject.toml), following semantic versioning
+   [./pyproject.toml](https://github.com/realazthat/mdremotifier/blob/v0.3.2/pyproject.toml), following semantic versioning
    principles. Also modify the `last_unstable_release` and `last_stable_release`
    in the `[tool.mdremotifier-project-metadata]` table as appropriate. Run
    `bash ./scripts/pre.sh` to ensure everything is in order.
 3. In the `develop` branch, commit these changes with a message like
    `"Prepare release X.Y.Z"`. (See the contributions section
    [above](#commit-process)).
 4. Merge the `develop` branch into the `master` branch:
@@ -295,35 +298,35 @@
 7. Push to GitHub: Push the commit and tags to GitHub with
    `git push && git push --tags`.
 8. The `--no-ff` option adds a commit to the master branch for the merge, so
    refork the develop branch from the master branch:
    `git checkout develop && git merge master`.
 9. Push the develop branch to GitHub: `git push origin develop`.
 
-[1]: https://raw.githubusercontent.com/realazthat/mdremotifier/v0.3.1/.github/logo-exported.svg
+[1]: https://raw.githubusercontent.com/realazthat/mdremotifier/v0.3.2/.github/logo-exported.svg
 [2]: https://img.shields.io/badge/Audience-Developers-0A1E1E?style=plastic&logo=data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIyNCIgaGVpZ2h0PSIyNCIgdmlld0JveD0iMCAwIDI0IDI0IiBmaWxsPSJub25lIiBzdHJva2U9ImN1cnJlbnRDb2xvciIgc3Ryb2tlLXdpZHRoPSIyIiBzdHJva2UtbGluZWNhcD0icm91bmQiIHN0cm9rZS1saW5lam9pbj0icm91bmQiIGNsYXNzPSJsdWNpZGUgbHVjaWRlLXVzZXJzIj48cGF0aCBkPSJNMTYgMjF2LTJhNCA0IDAgMCAwLTQtNEg2YTQgNCAwIDAgMC00IDR2MiIvPjxjaXJjbGUgY3g9IjkiIGN5PSI3IiByPSI0Ii8+PHBhdGggZD0iTTIyIDIxdi0yYTQgNCAwIDAgMC0zLTMuODciLz48cGF0aCBkPSJNMTYgMy4xM2E0IDQgMCAwIDEgMCA3Ljc1Ii8+PC9zdmc+
 [3]: https://img.shields.io/badge/Platform-Linux-0A1E1E?style=plastic&logo=data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIyNCIgaGVpZ2h0PSIyNCIgdmlld0JveD0iMCAwIDI0IDI0IiBmaWxsPSJub25lIiBzdHJva2U9ImN1cnJlbnRDb2xvciIgc3Ryb2tlLXdpZHRoPSIyIiBzdHJva2UtbGluZWNhcD0icm91bmQiIHN0cm9rZS1saW5lam9pbj0icm91bmQiIGNsYXNzPSJsdWNpZGUgbHVjaWRlLWxhcHRvcC1taW5pbWFsIj48cmVjdCB3aWR0aD0iMTgiIGhlaWdodD0iMTIiIHg9IjMiIHk9IjQiIHJ4PSIyIiByeT0iMiIvPjxsaW5lIHgxPSIyIiB4Mj0iMjIiIHkxPSIyMCIgeTI9IjIwIi8+PC9zdmc+
 [4]: https://img.shields.io/github/languages/top/realazthat/mdremotifier.svg?&cacheSeconds=28800&style=plastic&color=0A1E1E
 [5]: https://img.shields.io/github/license/realazthat/mdremotifier?style=plastic&color=0A1E1E
-[6]: https://github.com/realazthat/mdremotifier/blob/v0.3.1/LICENSE.md
+[6]: https://github.com/realazthat/mdremotifier/blob/v0.3.2/LICENSE.md
 [7]: https://img.shields.io/pypi/v/mdremotifier?style=plastic&color=0A1E1E
 [8]: https://pypi.org/project/mdremotifier/
 [9]: https://img.shields.io/pypi/pyversions/mdremotifier?style=plastic&color=0A1E1E
 [10]: https://github.com/realazthat/mdremotifier/tree/master
 [11]: https://img.shields.io/github/actions/workflow/status/realazthat/mdremotifier/build-and-test.yml?branch=master&style=plastic
 [12]: https://github.com/realazthat/mdremotifier/actions/workflows/build-and-test.yml
-[13]: https://img.shields.io/github/commits-since/realazthat/mdremotifier/v0.3.1/master?style=plastic
-[14]: https://github.com/realazthat/mdremotifier/compare/v0.3.1...master
+[13]: https://img.shields.io/github/commits-since/realazthat/mdremotifier/v0.3.2/master?style=plastic
+[14]: https://github.com/realazthat/mdremotifier/compare/v0.3.2...master
 [15]: https://img.shields.io/github/last-commit/realazthat/mdremotifier/master?style=plastic
 [16]: https://github.com/realazthat/mdremotifier/tree/develop
 [17]: https://img.shields.io/github/actions/workflow/status/realazthat/mdremotifier/build-and-test.yml?branch=develop&style=plastic
-[18]: https://img.shields.io/github/commits-since/realazthat/mdremotifier/v0.3.1/develop?style=plastic
-[19]: https://github.com/realazthat/mdremotifier/compare/v0.3.1...develop
-[20]: https://img.shields.io/github/commits-since/realazthat/mdremotifier/v0.3.1/develop?style=plastic
-[21]: https://github.com/realazthat/mdremotifier/compare/v0.3.1...develop
+[18]: https://img.shields.io/github/commits-since/realazthat/mdremotifier/v0.3.2/develop?style=plastic
+[19]: https://github.com/realazthat/mdremotifier/compare/v0.3.2...develop
+[20]: https://img.shields.io/github/commits-since/realazthat/mdremotifier/v0.3.2/develop?style=plastic
+[21]: https://github.com/realazthat/mdremotifier/compare/v0.3.2...develop
 [22]: https://img.shields.io/github/last-commit/realazthat/mdremotifier/develop?style=plastic
 [23]: https://github.com/bdashore3/remark-github-images "Documentation is non-existent, but code looks very similar to mdremotifier"
 [24]: https://github.com/laobie/WriteMarkdownLazily "Uploads to cloud."
 [25]: https://github.com/crh19970307/mdul "Uploads to sm.ms"
 [26]: https://github.com/SkyLee424/Go-MarkDown-Image-Transfer-Helper "Upload to Qiniu Cloud"
 [27]: https://github.com/jen6/imgo "Upload to Google Drive"
 [28]: https://github.com/chocoluffy/lazy-markdown "Uploads to LeanCloud, readme is a bit unclear"
```

#### html2text {}

```diff
@@ -9,148 +9,149 @@
 ---
 | | Status | Stable | Unstable | | | ----------------- | ----------------------
 ----- | ------------------------- | ------------------------- | ---------------
 --- | | **[Master][10]** | [![Build and Test][11]][12] | [![since tagged][13]]
 [14] | | ![last commit][15] | | **[Develop][16]** | [![Build and Test][17]][12]
 | [![since tagged][18]][19] | [![since tagged][20]][21] | ![last commit][22] |
 [Demo]## â What What mdremotifier does: Turn this ([./mdremotifier/examples/
-EXAMPLE.md](https://github.com/realazthat/mdremotifier/blob/v0.3.1/
+EXAMPLE.md](https://github.com/realazthat/mdremotifier/blob/v0.3.2/
 mdremotifier/examples/EXAMPLE.md)): ```md # Example markdown file A link to a
 local file [LICENSE.md](./LICENSE.md). ``` Into this ([./mdremotifier/examples/
-EXAMPLE.remotified.md](https://github.com/realazthat/mdremotifier/blob/v0.3.1/
+EXAMPLE.remotified.md](https://github.com/realazthat/mdremotifier/blob/v0.3.2/
 mdremotifier/examples/EXAMPLE.remotified.md)): ```md # Example markdown file A
 link to a local file [LICENSE.md](https://raw.githubusercontent.com/realazthat/
 mdremotifier/master/LICENSE.md). ``` This is useful for uploading `README.md`
 files to third-party sites, like the npmjs.com registry, or pypi.org registry,
 because these registries will break the local images in your README when
-displayed on their sites. ## ð Features - ð·ðð¡ðð¼ï¸ Replace
-local URLs with raw.githubusercontent.com URLs. ## ð  Installation ```bash #
-Install from pypi (https://pypi.org/project/mdremotifier/) pip install
-mdremotifier # Install from git (https://github.com/realazthat/mdremotifier)
-pip install git+https://github.com/realazthat/mdremotifier.git@v0.3.1 ``` ##
-ð Usage Example README: ([./mdremotifier/examples/EXAMPLE.md](https://
-github.com/realazthat/mdremotifier/blob/v0.3.1/mdremotifier/examples/
-EXAMPLE.md)): ```md # Example markdown file A link to a local file [LICENSE.md]
-(./LICENSE.md). ``` Generating the README: ```bash $ python -m mdremotifier.cli
--i ./mdremotifier/examples/EXAMPLE.md --url-prefix https://
-raw.githubusercontent.com/realazthat/mdremotifier/master/ -o - 2>/dev/null #
-Example markdown file A link to a local file [LICENSE.md](https://
-raw.githubusercontent.com/realazthat/mdremotifier/master/LICENSE.md). ``` ##
-ð» Command Line Options [Output of `python -m mdremotifier.cli --help`]##
-ð¡ Examples - mdremotifier's own `README`: - Original: [./README.md](https://
-github.com/realazthat/mdremotifier/blob/v0.3.1/README.md). - Remotified:
-[./.github/README.remotified.md](https://github.com/realazthat/mdremotifier/
-blob/v0.3.1/.github/README.remotified.md). - Generation script: [./scripts/
-generate-readme.sh](https://github.com/realazthat/mdremotifier/blob/v0.3.1/
-scripts/generate-readme.sh). - Example: - Original: [./mdremotifier/examples/
-EXAMPLE.md](https://github.com/realazthat/mdremotifier/blob/v0.3.1/
-mdremotifier/examples/EXAMPLE.md). - Remotified: [./mdremotifier/examples/
-EXAMPLE.remotified.md](https://github.com/realazthat/mdremotifier/blob/v0.3.1/
-mdremotifier/examples/EXAMPLE.remotified.md). - Generation script: [./
-mdremotifier/examples/example.sh](https://github.com/realazthat/mdremotifier/
-blob/v0.3.1/mdremotifier/examples/example.sh). ## â Requirements - Linux-like
-environment - Why: Uses pexpect.spawn(). - Python 3.8+ - Why: Some dev
-dependencies require Python 3.8+. ### Tested Platforms - WSL2 Ubuntu 20.04,
-Python `3.8.0`. - Ubuntu 20.04, Python `3.8.0, 3.9.0, 3.10.0, 3.11.0, 3.12.0`,
-tested in GitHub Actions workflow ([build-and-test.yml](https://github.com/
-realazthat/mdremotifier/blob/v0.3.1/.github/workflows/build-and-test.yml)). ##
-ð¤ Versioning We use SemVer for versioning. For the versions available, see
-the tags on this repository. ## ð License This project is licensed under the
-MIT License - see the [./LICENSE.md](https://github.com/realazthat/
-mdremotifier/blob/v0.3.1/LICENSE.md) file for details. ## ð Thanks Main
-libraries used in mdremotifier are: - Markdown AST: [mistletoe](https://
-github.com/miyuchina/mistletoe). - Colorful CLI help: [rich-argparse](https://
-github.com/hamdanal/rich-argparse). ## ð¤ Related Projects Not complete, and
-not necessarily up to date. Make a PR ([contributions](#-contributions)) to
-insert/modify. | Project | Stars | Last Update | Language | Platform |
-Similarity X Obviousness | | ------------------------------------------------
-- | ----- | ------------ | -------- | -------- | ------------------------ | |
-[bdashore3/remark-github-images][23] | 0 | `2022/12/29` | JS | CLI |
-â­â­â­â­â­ | | [laobie/WriteMarkdownLazily][24] | 36 | `2024/01/06` |
-Python | CLI | â­â­â­â­ | | [crh19970307/mdul][25] | 1 | `2020/02/01` |
-Python | CLI | â­â­â­â­ | | [SkyLee424/Go-MarkDown-Image-Transfer-Helper]
-[26] | 0 | `2024/03/25` | Go | CLI | â­â­â­â­ | | [jen6/imgo][27] | 0 |
-`2020/03/18` | Pyhon | CLI | â­â­â­â­ | | [chocoluffy/lazy-markdown][28] |
-0 | `2016/11/20` | Python | CLI | â­â­â­â­ | | [loheagn/gopic][29] | 0 |
-`2021/11/24` | Go | CLI | â­â­â­â­ | | [Undertone0809/imarkdown][30] | 57 |
-`2024/01/06` | Python | Python | â­â­â­ | | [ravgeetdhillon/markdown-imgur-
-upload][31] | 1 | `2022/03/26` | Python | CLI | â­â­â­ | ## ð«¡
-Contributions ### Development environment: Linux-like - For running `pre.sh`
-(Linux-like environment). - From [./.github/dependencies.yml](https://
-github.com/realazthat/mdremotifier/blob/v0.3.1/.github/dependencies.yml), which
-is used for the GH Action to do a fresh install of everything: ```yaml bash:
-scripts. findutils: scripts. grep: tests. xxd: tests. git: scripts, tests.
-xxhash: scripts (changeguard). rsync: out-of-directory test. expect: for
-`unbuffer`, useful to grab and compare ansi color symbols. jq: dependency for
-[yq](https://github.com/kislyuk/yq), which is used to generate the README; the
-README generator needs to use `tomlq` (which is a part of `yq`) to query
-`pyproject.toml`. ``` - Requires `pyenv`, or an exact matching version of
-python as in [.python-version](https://github.com/realazthat/mdremotifier/blob/
-v0.3.1/.python-version) (which is currently `3.8.0 `). - `jq`, ([installation]
-(https://jqlang.github.io/jq/)) required for [yq](https://github.com/kislyuk/
-yq), which is itself required for our [./README.md](https://github.com/
-realazthat/mdremotifier/blob/v0.3.1/README.md) generation, which uses `tomlq`
-(from the [yq](https://github.com/kislyuk/yq) package) to include version
-strings from [./pyproject.toml](https://github.com/realazthat/mdremotifier/
-blob/v0.3.1/pyproject.toml). - act (to run the GH Action locally): - Requires
-nodejs. - Requires Go. - docker. - Generate animation: - docker ### Commit
-Process 1. (Optionally) Fork the `develop` branch. 2. Stage your files: `git
-add path/to/file.py`. 3. `bash ./scripts/pre.sh`, this will format, lint, and
-test the code. 4. `git status` check if anything changed (generated [./
-README.md](https://github.com/realazthat/mdremotifier/blob/v0.3.1/README.md)
+displayed on their sites. See
+pypi.org/project/mdremotifier/>, notice how all of the images are not broken.
+## ð Features - ð·ðð¡ðð¼ï¸ Replace local URLs with
+raw.githubusercontent.com URLs. ## ð  Installation ```bash # Install from
+pypi (https://pypi.org/project/mdremotifier/) pip install mdremotifier #
+Install from git (https://github.com/realazthat/mdremotifier) pip install
+git+https://github.com/realazthat/mdremotifier.git@v0.3.2 ``` ## ð Usage
+Example README: ([./mdremotifier/examples/EXAMPLE.md](https://github.com/
+realazthat/mdremotifier/blob/v0.3.2/mdremotifier/examples/EXAMPLE.md)): ```md #
+Example markdown file A link to a local file [LICENSE.md](./LICENSE.md). ```
+Generating the README: ```bash $ python -m mdremotifier.cli -i ./mdremotifier/
+examples/EXAMPLE.md --url-prefix https://raw.githubusercontent.com/realazthat/
+mdremotifier/master/ -o - 2>/dev/null # Example markdown file A link to a local
+file [LICENSE.md](https://raw.githubusercontent.com/realazthat/mdremotifier/
+master/LICENSE.md). ``` ## ð» Command Line Options [Output of `python -
+m mdremotifier.cli --help`]## ð¡ Examples - mdremotifier's own `README`: -
+Original: [./README.md](https://github.com/realazthat/mdremotifier/blob/v0.3.2/
+README.md). - Remotified: [./.github/README.remotified.md](https://github.com/
+realazthat/mdremotifier/blob/v0.3.2/.github/README.remotified.md). - Generation
+script: [./scripts/generate-readme.sh](https://github.com/realazthat/
+mdremotifier/blob/v0.3.2/scripts/generate-readme.sh). - Example: - Original:
+[./mdremotifier/examples/EXAMPLE.md](https://github.com/realazthat/
+mdremotifier/blob/v0.3.2/mdremotifier/examples/EXAMPLE.md). - Remotified: [./
+mdremotifier/examples/EXAMPLE.remotified.md](https://github.com/realazthat/
+mdremotifier/blob/v0.3.2/mdremotifier/examples/EXAMPLE.remotified.md). -
+Generation script: [./mdremotifier/examples/example.sh](https://github.com/
+realazthat/mdremotifier/blob/v0.3.2/mdremotifier/examples/example.sh). ## â
+Requirements - Linux-like environment - Why: Uses pexpect.spawn(). - Python
+3.8+ - Why: Some dev dependencies require Python 3.8+. ### Tested Platforms -
+WSL2 Ubuntu 20.04, Python `3.8.0`. - Ubuntu 20.04, Python `3.8.0, 3.9.0,
+3.10.0, 3.11.0, 3.12.0`, tested in GitHub Actions workflow ([build-and-
+test.yml](https://github.com/realazthat/mdremotifier/blob/v0.3.2/.github/
+workflows/build-and-test.yml)). ## ð¤ Versioning We use SemVer for
+versioning. For the versions available, see the tags on this repository. ##
+ð License This project is licensed under the MIT License - see the [./
+LICENSE.md](https://github.com/realazthat/mdremotifier/blob/v0.3.2/LICENSE.md)
+file for details. ## ð Thanks Main libraries used in mdremotifier are: -
+Markdown AST: [mistletoe](https://github.com/miyuchina/mistletoe). - Colorful
+CLI help: [rich-argparse](https://github.com/hamdanal/rich-argparse). ## ð¤
+Related Projects Not complete, and not necessarily up to date. Make a PR (
+[contributions](#-contributions)) to insert/modify. | Project | Stars | Last
+Update | Language | Platform | Similarity X Obviousness | | -------------------
+------------------------------ | ----- | ------------ | -------- | -------- | -
+----------------------- | | [bdashore3/remark-github-images][23] | 0 | `2022/
+12/29` | JS | CLI | â­â­â­â­â­ | | [laobie/WriteMarkdownLazily][24] | 36 |
+`2024/01/06` | Python | CLI | â­â­â­â­ | | [crh19970307/mdul][25] | 1 |
+`2020/02/01` | Python | CLI | â­â­â­â­ | | [SkyLee424/Go-MarkDown-Image-
+Transfer-Helper][26] | 0 | `2024/03/25` | Go | CLI | â­â­â­â­ | | [jen6/
+imgo][27] | 0 | `2020/03/18` | Pyhon | CLI | â­â­â­â­ | | [chocoluffy/lazy-
+markdown][28] | 0 | `2016/11/20` | Python | CLI | â­â­â­â­ | | [loheagn/
+gopic][29] | 0 | `2021/11/24` | Go | CLI | â­â­â­â­ | | [Undertone0809/
+imarkdown][30] | 57 | `2024/01/06` | Python | Python | â­â­â­ | |
+[ravgeetdhillon/markdown-imgur-upload][31] | 1 | `2022/03/26` | Python | CLI |
+â­â­â­ | ## ð«¡ Contributions ### Development environment: Linux-like - For
+running `pre.sh` (Linux-like environment). - From [./.github/dependencies.yml]
+(https://github.com/realazthat/mdremotifier/blob/v0.3.2/.github/
+dependencies.yml), which is used for the GH Action to do a fresh install of
+everything: ```yaml bash: scripts. findutils: scripts. grep: tests. xxd: tests.
+git: scripts, tests. xxhash: scripts (changeguard). rsync: out-of-directory
+test. expect: for `unbuffer`, useful to grab and compare ansi color symbols.
+jq: dependency for [yq](https://github.com/kislyuk/yq), which is used to
+generate the README; the README generator needs to use `tomlq` (which is a part
+of `yq`) to query `pyproject.toml`. ``` - Requires `pyenv`, or an exact
+matching version of python as in [.python-version](https://github.com/
+realazthat/mdremotifier/blob/v0.3.2/.python-version) (which is currently `3.8.0
+`). - `jq`, ([installation](https://jqlang.github.io/jq/)) required for [yq]
+(https://github.com/kislyuk/yq), which is itself required for our [./README.md]
+(https://github.com/realazthat/mdremotifier/blob/v0.3.2/README.md) generation,
+which uses `tomlq` (from the [yq](https://github.com/kislyuk/yq) package) to
+include version strings from [./pyproject.toml](https://github.com/realazthat/
+mdremotifier/blob/v0.3.2/pyproject.toml). - act (to run the GH Action locally):
+- Requires nodejs. - Requires Go. - docker. - Generate animation: - docker ###
+Commit Process 1. (Optionally) Fork the `develop` branch. 2. Stage your files:
+`git add path/to/file.py`. 3. `bash ./scripts/pre.sh`, this will format, lint,
+and test the code. 4. `git status` check if anything changed (generated [./
+README.md](https://github.com/realazthat/mdremotifier/blob/v0.3.2/README.md)
 for example), if so, `git add` the changes, and go back to the previous step.
 5. `git commit -m "..."`. 6. Make a PR to `develop` (or push to develop if you
 have the rights). ## ðð Release Process These instructions are for
 maintainers of the project. 1. In the `develop` branch, run `bash ./scripts/
 pre.sh` to ensure everything is in order. 2. In the `develop` branch, bump the
 version in [./pyproject.toml](https://github.com/realazthat/mdremotifier/blob/
-v0.3.1/pyproject.toml), following semantic versioning principles. Also modify
+v0.3.2/pyproject.toml), following semantic versioning principles. Also modify
 the `last_unstable_release` and `last_stable_release` in the `
 [tool.mdremotifier-project-metadata]` table as appropriate. Run `bash ./
 scripts/pre.sh` to ensure everything is in order. 3. In the `develop` branch,
 commit these changes with a message like `"Prepare release X.Y.Z"`. (See the
 contributions section [above](#commit-process)). 4. Merge the `develop` branch
 into the `master` branch: `git checkout master && git merge develop --no-ff`.
 5. `master` branch: Tag the release: Create a git tag for the release with `git
 tag -a vX.Y.Z -m "Version X.Y.Z"`. 6. Publish to PyPI: Publish the release to
 PyPI with `bash ./scripts/deploy-to-pypi.sh`. 7. Push to GitHub: Push the
 commit and tags to GitHub with `git push && git push --tags`. 8. The `--no-ff`
 option adds a commit to the master branch for the merge, so refork the develop
 branch from the master branch: `git checkout develop && git merge master`. 9.
 Push the develop branch to GitHub: `git push origin develop`. [1]: https://
-raw.githubusercontent.com/realazthat/mdremotifier/v0.3.1/.github/logo-
+raw.githubusercontent.com/realazthat/mdremotifier/v0.3.2/.github/logo-
 exported.svg [2]: https://img.shields.io/badge/Audience-Developers-
 0A1E1E?style=plastic&logo=data:image/
 svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIyNCIgaGVpZ2h0PSIyNCIgdmlld0JveD0iMCAwIDI0IDI0IiBmaWxsPSJub25lIiBzdHJva2U9ImN1cnJlbnRDb2xvciIgc3Ryb2tlLXdpZHRoPSIyIiBzdHJva2UtbGluZWNhcD0icm91bmQiIHN0cm9rZS1saW5lam9pbj0icm91bmQiIGNsYXNzPSJsdWNpZGUgbHVjaWRlLXVzZXJzIj48cGF0aCBkPSJNMTYgMjF2LTJhNCA0IDAgMCAwLTQtNEg2YTQgNCAwIDAgMC00IDR2MiIvPjxjaXJjbGUgY3g9IjkiIGN5PSI3IiByPSI0Ii8+PHBhdGggZD0iTTIyIDIxdi0yYTQgNCAwIDAgMC0zLTMuODciLz48cGF0aCBkPSJNMTYgMy4xM2E0IDQgMCAwIDEgMCA3Ljc1Ii8+PC9zdmc+
 [3]: https://img.shields.io/badge/Platform-Linux-
 0A1E1E?style=plastic&logo=data:image/
 svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIyNCIgaGVpZ2h0PSIyNCIgdmlld0JveD0iMCAwIDI0IDI0IiBmaWxsPSJub25lIiBzdHJva2U9ImN1cnJlbnRDb2xvciIgc3Ryb2tlLXdpZHRoPSIyIiBzdHJva2UtbGluZWNhcD0icm91bmQiIHN0cm9rZS1saW5lam9pbj0icm91bmQiIGNsYXNzPSJsdWNpZGUgbHVjaWRlLWxhcHRvcC1taW5pbWFsIj48cmVjdCB3aWR0aD0iMTgiIGhlaWdodD0iMTIiIHg9IjMiIHk9IjQiIHJ4PSIyIiByeT0iMiIvPjxsaW5lIHgxPSIyIiB4Mj0iMjIiIHkxPSIyMCIgeTI9IjIwIi8+PC9zdmc+
 [4]: https://img.shields.io/github/languages/top/realazthat/
 mdremotifier.svg?&cacheSeconds=28800&style=plastic&color=0A1E1E [5]: https://
 img.shields.io/github/license/realazthat/
 mdremotifier?style=plastic&color=0A1E1E [6]: https://github.com/realazthat/
-mdremotifier/blob/v0.3.1/LICENSE.md [7]: https://img.shields.io/pypi/v/
+mdremotifier/blob/v0.3.2/LICENSE.md [7]: https://img.shields.io/pypi/v/
 mdremotifier?style=plastic&color=0A1E1E [8]: https://pypi.org/project/
 mdremotifier/ [9]: https://img.shields.io/pypi/pyversions/
 mdremotifier?style=plastic&color=0A1E1E [10]: https://github.com/realazthat/
 mdremotifier/tree/master [11]: https://img.shields.io/github/actions/workflow/
 status/realazthat/mdremotifier/build-and-test.yml?branch=master&style=plastic
 [12]: https://github.com/realazthat/mdremotifier/actions/workflows/build-and-
 test.yml [13]: https://img.shields.io/github/commits-since/realazthat/
-mdremotifier/v0.3.1/master?style=plastic [14]: https://github.com/realazthat/
-mdremotifier/compare/v0.3.1...master [15]: https://img.shields.io/github/last-
+mdremotifier/v0.3.2/master?style=plastic [14]: https://github.com/realazthat/
+mdremotifier/compare/v0.3.2...master [15]: https://img.shields.io/github/last-
 commit/realazthat/mdremotifier/master?style=plastic [16]: https://github.com/
 realazthat/mdremotifier/tree/develop [17]: https://img.shields.io/github/
 actions/workflow/status/realazthat/mdremotifier/build-and-
 test.yml?branch=develop&style=plastic [18]: https://img.shields.io/github/
-commits-since/realazthat/mdremotifier/v0.3.1/develop?style=plastic [19]: https:
-//github.com/realazthat/mdremotifier/compare/v0.3.1...develop [20]: https://
-img.shields.io/github/commits-since/realazthat/mdremotifier/v0.3.1/
+commits-since/realazthat/mdremotifier/v0.3.2/develop?style=plastic [19]: https:
+//github.com/realazthat/mdremotifier/compare/v0.3.2...develop [20]: https://
+img.shields.io/github/commits-since/realazthat/mdremotifier/v0.3.2/
 develop?style=plastic [21]: https://github.com/realazthat/mdremotifier/compare/
-v0.3.1...develop [22]: https://img.shields.io/github/last-commit/realazthat/
+v0.3.2...develop [22]: https://img.shields.io/github/last-commit/realazthat/
 mdremotifier/develop?style=plastic [23]: https://github.com/bdashore3/remark-
 github-images "Documentation is non-existent, but code looks very similar to
 mdremotifier" [24]: https://github.com/laobie/WriteMarkdownLazily "Uploads to
 cloud." [25]: https://github.com/crh19970307/mdul "Uploads to sm.ms" [26]:
 https://github.com/SkyLee424/Go-MarkDown-Image-Transfer-Helper "Upload to Qiniu
 Cloud" [27]: https://github.com/jen6/imgo "Upload to Google Drive" [28]: https:
 //github.com/chocoluffy/lazy-markdown "Uploads to LeanCloud, readme is a bit
```

### Comparing `mdremotifier-0.3.1/LICENSE.md` & `mdremotifier-0.3.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `mdremotifier-0.3.1/PKG-INFO` & `mdremotifier-0.3.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mdremotifier
-Version: 0.3.1
+Version: 0.3.2
 Summary: Remotify local links in README.md.
 Author-email: AYF <realazthat@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Azriel Fasten.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
@@ -91,14 +91,15 @@
 Requires-Dist: jaraco-functools==4.0.1; extra == "dev"
 Requires-Dist: jeepney==0.8.0; extra == "dev"
 Requires-Dist: jinja2==3.1.3; extra == "dev"
 Requires-Dist: keyring==25.2.0; extra == "dev"
 Requires-Dist: markdown-it-py==3.0.0; extra == "dev"
 Requires-Dist: markupsafe==2.1.5; extra == "dev"
 Requires-Dist: mdurl==0.1.2; extra == "dev"
+Requires-Dist: mdreftidy==0.3.0; extra == "dev"
 Requires-Dist: mistletoe==1.3.0; extra == "dev"
 Requires-Dist: more-itertools==10.2.0; extra == "dev"
 Requires-Dist: mypy==1.8.0; extra == "dev"
 Requires-Dist: mypy-extensions==1.0.0; extra == "dev"
 Requires-Dist: nh3==0.2.17; extra == "dev"
 Requires-Dist: nodeenv==1.8.0; extra == "dev"
 Requires-Dist: pathspec==0.12.1; extra == "dev"
@@ -201,64 +202,67 @@
 |                   | Status                      | Stable                    | Unstable                  |                    |
 | ----------------- | --------------------------- | ------------------------- | ------------------------- | ------------------ |
 | **[Master][10]**  | [![Build and Test][11]][12] | [![since tagged][13]][14] |                           | ![last commit][15] |
 | **[Develop][16]** | [![Build and Test][17]][12] | [![since tagged][18]][19] | [![since tagged][20]][21] | ![last commit][22] |
 
 </div>
 
-<img alt="Demo" src="https://raw.githubusercontent.com/realazthat/mdremotifier/v0.3.1/.github/demo.gif" width="100%"/>
+<img alt="Demo" src="https://raw.githubusercontent.com/realazthat/mdremotifier/v0.3.2/.github/demo.gif" width="100%"/>
 
 ## ❔ What
 
 What mdremotifier does:
 
-Turn this ([./mdremotifier/examples/EXAMPLE.md](https://github.com/realazthat/mdremotifier/blob/v0.3.1/mdremotifier/examples/EXAMPLE.md)):
+Turn this ([./mdremotifier/examples/EXAMPLE.md](https://github.com/realazthat/mdremotifier/blob/v0.3.2/mdremotifier/examples/EXAMPLE.md)):
 
 <!---->
 ```md
 # Example markdown file
 
 A link to a local file [LICENSE.md](./LICENSE.md).
 
 ```
 <!---->
 
 Into this
-([./mdremotifier/examples/EXAMPLE.remotified.md](https://github.com/realazthat/mdremotifier/blob/v0.3.1/mdremotifier/examples/EXAMPLE.remotified.md)):
+([./mdremotifier/examples/EXAMPLE.remotified.md](https://github.com/realazthat/mdremotifier/blob/v0.3.2/mdremotifier/examples/EXAMPLE.remotified.md)):
 
 <!---->
 ```md
 # Example markdown file
 
 A link to a local file [LICENSE.md](https://raw.githubusercontent.com/realazthat/mdremotifier/master/LICENSE.md).
 
 ```
 <!---->
 
 This is useful for uploading `README.md` files to third-party sites, like the
 npmjs.com registry, or pypi.org registry, because these registries will break
 the local images in your README when displayed on their sites.
 
+See <https://pypi.org/project/mdremotifier/>, notice how all of the images are
+not broken.
+
 ## 🎇 Features
 
 - 📷🔗📡🌐🖼️ Replace local URLs with raw.githubusercontent.com URLs.
 
 ## 🏠 Installation
 
 ```bash
 # Install from pypi (https://pypi.org/project/mdremotifier/)
 pip install mdremotifier
 
 # Install from git (https://github.com/realazthat/mdremotifier)
-pip install git+https://github.com/realazthat/mdremotifier.git@v0.3.1
+pip install git+https://github.com/realazthat/mdremotifier.git@v0.3.2
 ```
 
 ## 🚜 Usage
 
-Example README: ([./mdremotifier/examples/EXAMPLE.md](https://github.com/realazthat/mdremotifier/blob/v0.3.1/mdremotifier/examples/EXAMPLE.md)):
+Example README: ([./mdremotifier/examples/EXAMPLE.md](https://github.com/realazthat/mdremotifier/blob/v0.3.2/mdremotifier/examples/EXAMPLE.md)):
 
 <!---->
 ```md
 # Example markdown file
 
 A link to a local file [LICENSE.md](./LICENSE.md).
 
@@ -276,29 +280,29 @@
 
 ```
 <!---->
 
 ## 💻 Command Line Options
 
 <!---->
-<img alt="Output of `python -m mdremotifier.cli --help`" src="https://raw.githubusercontent.com/realazthat/mdremotifier/v0.3.1/README.help.generated.svg"/>
+<img alt="Output of `python -m mdremotifier.cli --help`" src="https://raw.githubusercontent.com/realazthat/mdremotifier/v0.3.2/README.help.generated.svg"/>
 <!-- -->
 
 ## 💡 Examples
 
 - mdremotifier's own `README`:
-  - Original: [./README.md](https://github.com/realazthat/mdremotifier/blob/v0.3.1/README.md).
-  - Remotified: [./.github/README.remotified.md](https://github.com/realazthat/mdremotifier/blob/v0.3.1/.github/README.remotified.md).
-  - Generation script: [./scripts/generate-readme.sh](https://github.com/realazthat/mdremotifier/blob/v0.3.1/scripts/generate-readme.sh).
+  - Original: [./README.md](https://github.com/realazthat/mdremotifier/blob/v0.3.2/README.md).
+  - Remotified: [./.github/README.remotified.md](https://github.com/realazthat/mdremotifier/blob/v0.3.2/.github/README.remotified.md).
+  - Generation script: [./scripts/generate-readme.sh](https://github.com/realazthat/mdremotifier/blob/v0.3.2/scripts/generate-readme.sh).
 - Example:
-  - Original: [./mdremotifier/examples/EXAMPLE.md](https://github.com/realazthat/mdremotifier/blob/v0.3.1/mdremotifier/examples/EXAMPLE.md).
+  - Original: [./mdremotifier/examples/EXAMPLE.md](https://github.com/realazthat/mdremotifier/blob/v0.3.2/mdremotifier/examples/EXAMPLE.md).
   - Remotified:
-    [./mdremotifier/examples/EXAMPLE.remotified.md](https://github.com/realazthat/mdremotifier/blob/v0.3.1/mdremotifier/examples/EXAMPLE.remotified.md).
+    [./mdremotifier/examples/EXAMPLE.remotified.md](https://github.com/realazthat/mdremotifier/blob/v0.3.2/mdremotifier/examples/EXAMPLE.remotified.md).
   - Generation script:
-    [./mdremotifier/examples/example.sh](https://github.com/realazthat/mdremotifier/blob/v0.3.1/mdremotifier/examples/example.sh).
+    [./mdremotifier/examples/example.sh](https://github.com/realazthat/mdremotifier/blob/v0.3.2/mdremotifier/examples/example.sh).
 
 <!-- TODO: Rebuild this for mdremotifier
 - Projects using mdremotifier:
   - [realazthat/snipinator](https://github.com/realazthat/snipinator), See
     [snipinator/README.md.jinja2](https://github.com/realazthat/snipinator/blob/61cb88593baa099dc375cf5fd40679e4be673fc5/README.md.jinja2).
   - [github.com/realazthat/changeguard](https://github.com/realazthat/changeguard),
     See
@@ -321,25 +325,25 @@
 - Python 3.8+
   - Why: Some dev dependencies require Python 3.8+.
 
 ### Tested Platforms
 
 - WSL2 Ubuntu 20.04, Python `3.8.0`.
 - Ubuntu 20.04, Python `3.8.0, 3.9.0, 3.10.0, 3.11.0, 3.12.0`, tested in GitHub Actions
-  workflow ([build-and-test.yml](https://github.com/realazthat/mdremotifier/blob/v0.3.1/.github/workflows/build-and-test.yml)).
+  workflow ([build-and-test.yml](https://github.com/realazthat/mdremotifier/blob/v0.3.2/.github/workflows/build-and-test.yml)).
 
 ## 🤏 Versioning
 
 We use SemVer for versioning. For the versions available, see the tags on this
 repository.
 
 ## 🔑 License
 
 This project is licensed under the MIT License - see the
-[./LICENSE.md](https://github.com/realazthat/mdremotifier/blob/v0.3.1/LICENSE.md) file for details.
+[./LICENSE.md](https://github.com/realazthat/mdremotifier/blob/v0.3.2/LICENSE.md) file for details.
 
 ## 🙏 Thanks
 
 Main libraries used in mdremotifier are:
 
 - Markdown AST: [mistletoe](https://github.com/miyuchina/mistletoe).
 - Colorful CLI help: [rich-argparse](https://github.com/hamdanal/rich-argparse).
@@ -363,15 +367,15 @@
 
 ## 🫡 Contributions
 
 ### Development environment: Linux-like
 
 - For running `pre.sh` (Linux-like environment).
 
-  - From [./.github/dependencies.yml](https://github.com/realazthat/mdremotifier/blob/v0.3.1/.github/dependencies.yml), which is used for
+  - From [./.github/dependencies.yml](https://github.com/realazthat/mdremotifier/blob/v0.3.2/.github/dependencies.yml), which is used for
     the GH Action to do a fresh install of everything:
 
     ```yaml
     bash: scripts.
     findutils: scripts.
     grep: tests.
     xxd: tests.
@@ -382,47 +386,47 @@
     jq: dependency for [yq](https://github.com/kislyuk/yq), which is used to generate
       the README; the README generator needs to use `tomlq` (which is a part of `yq`)
       to query `pyproject.toml`.
 
     ```
 
   - Requires `pyenv`, or an exact matching version of python as in
-    [.python-version](https://github.com/realazthat/mdremotifier/blob/v0.3.1/.python-version) (which is currently
+    [.python-version](https://github.com/realazthat/mdremotifier/blob/v0.3.2/.python-version) (which is currently
     `3.8.0 `).
   - `jq`, ([installation](https://jqlang.github.io/jq/)) required for
     [yq](https://github.com/kislyuk/yq), which is itself required for our
-    [./README.md](https://github.com/realazthat/mdremotifier/blob/v0.3.1/README.md) generation, which uses `tomlq` (from the
+    [./README.md](https://github.com/realazthat/mdremotifier/blob/v0.3.2/README.md) generation, which uses `tomlq` (from the
     [yq](https://github.com/kislyuk/yq) package) to include version strings from
-    [./pyproject.toml](https://github.com/realazthat/mdremotifier/blob/v0.3.1/pyproject.toml).
+    [./pyproject.toml](https://github.com/realazthat/mdremotifier/blob/v0.3.2/pyproject.toml).
   - act (to run the GH Action locally):
     - Requires nodejs.
     - Requires Go.
     - docker.
   - Generate animation:
     - docker
 
 ### Commit Process
 
 1. (Optionally) Fork the `develop` branch.
 2. Stage your files: `git add path/to/file.py`.
 3. `bash ./scripts/pre.sh`, this will format, lint, and test the code.
 4. `git status` check if anything changed (generated
-   [./README.md](https://github.com/realazthat/mdremotifier/blob/v0.3.1/README.md) for example), if so, `git add` the
+   [./README.md](https://github.com/realazthat/mdremotifier/blob/v0.3.2/README.md) for example), if so, `git add` the
    changes, and go back to the previous step.
 5. `git commit -m "..."`.
 6. Make a PR to `develop` (or push to develop if you have the rights).
 
 ## 🔄🚀 Release Process
 
 These instructions are for maintainers of the project.
 
 1. In the `develop` branch, run `bash ./scripts/pre.sh` to ensure
    everything is in order.
 2. In the `develop` branch, bump the version in
-   [./pyproject.toml](https://github.com/realazthat/mdremotifier/blob/v0.3.1/pyproject.toml), following semantic versioning
+   [./pyproject.toml](https://github.com/realazthat/mdremotifier/blob/v0.3.2/pyproject.toml), following semantic versioning
    principles. Also modify the `last_unstable_release` and `last_stable_release`
    in the `[tool.mdremotifier-project-metadata]` table as appropriate. Run
    `bash ./scripts/pre.sh` to ensure everything is in order.
 3. In the `develop` branch, commit these changes with a message like
    `"Prepare release X.Y.Z"`. (See the contributions section
    [above](#commit-process)).
 4. Merge the `develop` branch into the `master` branch:
@@ -434,35 +438,35 @@
 7. Push to GitHub: Push the commit and tags to GitHub with
    `git push && git push --tags`.
 8. The `--no-ff` option adds a commit to the master branch for the merge, so
    refork the develop branch from the master branch:
    `git checkout develop && git merge master`.
 9. Push the develop branch to GitHub: `git push origin develop`.
 
-[1]: https://raw.githubusercontent.com/realazthat/mdremotifier/v0.3.1/.github/logo-exported.svg
+[1]: https://raw.githubusercontent.com/realazthat/mdremotifier/v0.3.2/.github/logo-exported.svg
 [2]: https://img.shields.io/badge/Audience-Developers-0A1E1E?style=plastic&logo=data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIyNCIgaGVpZ2h0PSIyNCIgdmlld0JveD0iMCAwIDI0IDI0IiBmaWxsPSJub25lIiBzdHJva2U9ImN1cnJlbnRDb2xvciIgc3Ryb2tlLXdpZHRoPSIyIiBzdHJva2UtbGluZWNhcD0icm91bmQiIHN0cm9rZS1saW5lam9pbj0icm91bmQiIGNsYXNzPSJsdWNpZGUgbHVjaWRlLXVzZXJzIj48cGF0aCBkPSJNMTYgMjF2LTJhNCA0IDAgMCAwLTQtNEg2YTQgNCAwIDAgMC00IDR2MiIvPjxjaXJjbGUgY3g9IjkiIGN5PSI3IiByPSI0Ii8+PHBhdGggZD0iTTIyIDIxdi0yYTQgNCAwIDAgMC0zLTMuODciLz48cGF0aCBkPSJNMTYgMy4xM2E0IDQgMCAwIDEgMCA3Ljc1Ii8+PC9zdmc+
 [3]: https://img.shields.io/badge/Platform-Linux-0A1E1E?style=plastic&logo=data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIyNCIgaGVpZ2h0PSIyNCIgdmlld0JveD0iMCAwIDI0IDI0IiBmaWxsPSJub25lIiBzdHJva2U9ImN1cnJlbnRDb2xvciIgc3Ryb2tlLXdpZHRoPSIyIiBzdHJva2UtbGluZWNhcD0icm91bmQiIHN0cm9rZS1saW5lam9pbj0icm91bmQiIGNsYXNzPSJsdWNpZGUgbHVjaWRlLWxhcHRvcC1taW5pbWFsIj48cmVjdCB3aWR0aD0iMTgiIGhlaWdodD0iMTIiIHg9IjMiIHk9IjQiIHJ4PSIyIiByeT0iMiIvPjxsaW5lIHgxPSIyIiB4Mj0iMjIiIHkxPSIyMCIgeTI9IjIwIi8+PC9zdmc+
 [4]: https://img.shields.io/github/languages/top/realazthat/mdremotifier.svg?&cacheSeconds=28800&style=plastic&color=0A1E1E
 [5]: https://img.shields.io/github/license/realazthat/mdremotifier?style=plastic&color=0A1E1E
-[6]: https://github.com/realazthat/mdremotifier/blob/v0.3.1/LICENSE.md
+[6]: https://github.com/realazthat/mdremotifier/blob/v0.3.2/LICENSE.md
 [7]: https://img.shields.io/pypi/v/mdremotifier?style=plastic&color=0A1E1E
 [8]: https://pypi.org/project/mdremotifier/
 [9]: https://img.shields.io/pypi/pyversions/mdremotifier?style=plastic&color=0A1E1E
 [10]: https://github.com/realazthat/mdremotifier/tree/master
 [11]: https://img.shields.io/github/actions/workflow/status/realazthat/mdremotifier/build-and-test.yml?branch=master&style=plastic
 [12]: https://github.com/realazthat/mdremotifier/actions/workflows/build-and-test.yml
-[13]: https://img.shields.io/github/commits-since/realazthat/mdremotifier/v0.3.1/master?style=plastic
-[14]: https://github.com/realazthat/mdremotifier/compare/v0.3.1...master
+[13]: https://img.shields.io/github/commits-since/realazthat/mdremotifier/v0.3.2/master?style=plastic
+[14]: https://github.com/realazthat/mdremotifier/compare/v0.3.2...master
 [15]: https://img.shields.io/github/last-commit/realazthat/mdremotifier/master?style=plastic
 [16]: https://github.com/realazthat/mdremotifier/tree/develop
 [17]: https://img.shields.io/github/actions/workflow/status/realazthat/mdremotifier/build-and-test.yml?branch=develop&style=plastic
-[18]: https://img.shields.io/github/commits-since/realazthat/mdremotifier/v0.3.1/develop?style=plastic
-[19]: https://github.com/realazthat/mdremotifier/compare/v0.3.1...develop
-[20]: https://img.shields.io/github/commits-since/realazthat/mdremotifier/v0.3.1/develop?style=plastic
-[21]: https://github.com/realazthat/mdremotifier/compare/v0.3.1...develop
+[18]: https://img.shields.io/github/commits-since/realazthat/mdremotifier/v0.3.2/develop?style=plastic
+[19]: https://github.com/realazthat/mdremotifier/compare/v0.3.2...develop
+[20]: https://img.shields.io/github/commits-since/realazthat/mdremotifier/v0.3.2/develop?style=plastic
+[21]: https://github.com/realazthat/mdremotifier/compare/v0.3.2...develop
 [22]: https://img.shields.io/github/last-commit/realazthat/mdremotifier/develop?style=plastic
 [23]: https://github.com/bdashore3/remark-github-images "Documentation is non-existent, but code looks very similar to mdremotifier"
 [24]: https://github.com/laobie/WriteMarkdownLazily "Uploads to cloud."
 [25]: https://github.com/crh19970307/mdul "Uploads to sm.ms"
 [26]: https://github.com/SkyLee424/Go-MarkDown-Image-Transfer-Helper "Upload to Qiniu Cloud"
 [27]: https://github.com/jen6/imgo "Upload to Google Drive"
 [28]: https://github.com/chocoluffy/lazy-markdown "Uploads to LeanCloud, readme is a bit unclear"
```

### Comparing `mdremotifier-0.3.1/README.md` & `mdremotifier-0.3.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -95,26 +95,29 @@
 ```
 <!---->
 
 This is useful for uploading `README.md` files to third-party sites, like the
 npmjs.com registry, or pypi.org registry, because these registries will break
 the local images in your README when displayed on their sites.
 
+See <https://pypi.org/project/mdremotifier/>, notice how all of the images are
+not broken.
+
 ## 🎇 Features
 
 - 📷🔗📡🌐🖼️ Replace local URLs with raw.githubusercontent.com URLs.
 
 ## 🏠 Installation
 
 ```bash
 # Install from pypi (https://pypi.org/project/mdremotifier/)
 pip install mdremotifier
 
 # Install from git (https://github.com/realazthat/mdremotifier)
-pip install git+https://github.com/realazthat/mdremotifier.git@v0.3.1
+pip install git+https://github.com/realazthat/mdremotifier.git@v0.3.2
 ```
 
 ## 🚜 Usage
 
 Example README: ([./mdremotifier/examples/EXAMPLE.md](./mdremotifier/examples/EXAMPLE.md)):
 
 <!---->
@@ -317,30 +320,30 @@
   https://img.shields.io/pypi/pyversions/mdremotifier?style=plastic&color=0A1E1E
 [10]: https://github.com/realazthat/mdremotifier/tree/master
 [11]:
   https://img.shields.io/github/actions/workflow/status/realazthat/mdremotifier/build-and-test.yml?branch=master&style=plastic
 [12]:
   https://github.com/realazthat/mdremotifier/actions/workflows/build-and-test.yml
 [13]:
-  https://img.shields.io/github/commits-since/realazthat/mdremotifier/v0.3.1/master?style=plastic
+  https://img.shields.io/github/commits-since/realazthat/mdremotifier/v0.3.2/master?style=plastic
 [14]:
-  https://github.com/realazthat/mdremotifier/compare/v0.3.1...master
+  https://github.com/realazthat/mdremotifier/compare/v0.3.2...master
 [15]:
   https://img.shields.io/github/last-commit/realazthat/mdremotifier/master?style=plastic
 [16]: https://github.com/realazthat/mdremotifier/tree/develop
 [17]:
   https://img.shields.io/github/actions/workflow/status/realazthat/mdremotifier/build-and-test.yml?branch=develop&style=plastic
 [18]:
-  https://img.shields.io/github/commits-since/realazthat/mdremotifier/v0.3.1/develop?style=plastic
+  https://img.shields.io/github/commits-since/realazthat/mdremotifier/v0.3.2/develop?style=plastic
 [19]:
-  https://github.com/realazthat/mdremotifier/compare/v0.3.1...develop
+  https://github.com/realazthat/mdremotifier/compare/v0.3.2...develop
 [20]:
-  https://img.shields.io/github/commits-since/realazthat/mdremotifier/v0.3.1/develop?style=plastic
+  https://img.shields.io/github/commits-since/realazthat/mdremotifier/v0.3.2/develop?style=plastic
 [21]:
-  https://github.com/realazthat/mdremotifier/compare/v0.3.1...develop
+  https://github.com/realazthat/mdremotifier/compare/v0.3.2...develop
 [22]:
   https://img.shields.io/github/last-commit/realazthat/mdremotifier/develop?style=plastic
 [23]:
   https://github.com/bdashore3/remark-github-images
   "Documentation is non-existent, but code looks very similar to mdremotifier"
 [24]: https://github.com/laobie/WriteMarkdownLazily "Uploads to cloud."
 [25]: https://github.com/crh19970307/mdul "Uploads to sm.ms"
```

#### html2text {}

```diff
@@ -17,19 +17,21 @@
 A link to a local file [LICENSE.md](./LICENSE.md). ``` Into this ([./
 mdremotifier/examples/EXAMPLE.remotified.md](./mdremotifier/examples/
 EXAMPLE.remotified.md)): ```md # Example markdown file A link to a local file
 [LICENSE.md](https://raw.githubusercontent.com/realazthat/mdremotifier/master/
 LICENSE.md). ``` This is useful for uploading `README.md` files to third-party
 sites, like the npmjs.com registry, or pypi.org registry, because these
 registries will break the local images in your README when displayed on their
-sites. ## ð Features - ð·ðð¡ðð¼ï¸ Replace local URLs with
+sites. See
+pypi.org/project/mdremotifier/>, notice how all of the images are not broken.
+## ð Features - ð·ðð¡ðð¼ï¸ Replace local URLs with
 raw.githubusercontent.com URLs. ## ð  Installation ```bash # Install from
 pypi (https://pypi.org/project/mdremotifier/) pip install mdremotifier #
 Install from git (https://github.com/realazthat/mdremotifier) pip install
-git+https://github.com/realazthat/mdremotifier.git@v0.3.1 ``` ## ð Usage
+git+https://github.com/realazthat/mdremotifier.git@v0.3.2 ``` ## ð Usage
 Example README: ([./mdremotifier/examples/EXAMPLE.md](./mdremotifier/examples/
 EXAMPLE.md)): ```md # Example markdown file A link to a local file [LICENSE.md]
 (./LICENSE.md). ``` Generating the README: ```bash $ python -m mdremotifier.cli
 -i ./mdremotifier/examples/EXAMPLE.md --url-prefix https://
 raw.githubusercontent.com/realazthat/mdremotifier/master/ -o - 2>/dev/null #
 Example markdown file A link to a local file [LICENSE.md](https://
 raw.githubusercontent.com/realazthat/mdremotifier/master/LICENSE.md). ``` ##
@@ -118,25 +120,25 @@
 img.shields.io/pypi/v/mdremotifier?style=plastic&color=0A1E1E [8]: https://
 pypi.org/project/mdremotifier/ [9]: https://img.shields.io/pypi/pyversions/
 mdremotifier?style=plastic&color=0A1E1E [10]: https://github.com/realazthat/
 mdremotifier/tree/master [11]: https://img.shields.io/github/actions/workflow/
 status/realazthat/mdremotifier/build-and-test.yml?branch=master&style=plastic
 [12]: https://github.com/realazthat/mdremotifier/actions/workflows/build-and-
 test.yml [13]: https://img.shields.io/github/commits-since/realazthat/
-mdremotifier/v0.3.1/master?style=plastic [14]: https://github.com/realazthat/
-mdremotifier/compare/v0.3.1...master [15]: https://img.shields.io/github/last-
+mdremotifier/v0.3.2/master?style=plastic [14]: https://github.com/realazthat/
+mdremotifier/compare/v0.3.2...master [15]: https://img.shields.io/github/last-
 commit/realazthat/mdremotifier/master?style=plastic [16]: https://github.com/
 realazthat/mdremotifier/tree/develop [17]: https://img.shields.io/github/
 actions/workflow/status/realazthat/mdremotifier/build-and-
 test.yml?branch=develop&style=plastic [18]: https://img.shields.io/github/
-commits-since/realazthat/mdremotifier/v0.3.1/develop?style=plastic [19]: https:
-//github.com/realazthat/mdremotifier/compare/v0.3.1...develop [20]: https://
-img.shields.io/github/commits-since/realazthat/mdremotifier/v0.3.1/
+commits-since/realazthat/mdremotifier/v0.3.2/develop?style=plastic [19]: https:
+//github.com/realazthat/mdremotifier/compare/v0.3.2...develop [20]: https://
+img.shields.io/github/commits-since/realazthat/mdremotifier/v0.3.2/
 develop?style=plastic [21]: https://github.com/realazthat/mdremotifier/compare/
-v0.3.1...develop [22]: https://img.shields.io/github/last-commit/realazthat/
+v0.3.2...develop [22]: https://img.shields.io/github/last-commit/realazthat/
 mdremotifier/develop?style=plastic [23]: https://github.com/bdashore3/remark-
 github-images "Documentation is non-existent, but code looks very similar to
 mdremotifier" [24]: https://github.com/laobie/WriteMarkdownLazily "Uploads to
 cloud." [25]: https://github.com/crh19970307/mdul "Uploads to sm.ms" [26]:
 https://github.com/SkyLee424/Go-MarkDown-Image-Transfer-Helper "Upload to Qiniu
 Cloud" [27]: https://github.com/jen6/imgo "Upload to Google Drive" [28]: https:
 //github.com/chocoluffy/lazy-markdown "Uploads to LeanCloud, readme is a bit
```

### Comparing `mdremotifier-0.3.1/mdremotifier/cli.py` & `mdremotifier-0.3.2/mdremotifier/cli.py`

 * *Files identical despite different names*

### Comparing `mdremotifier-0.3.1/mdremotifier.egg-info/PKG-INFO` & `mdremotifier-0.3.2/mdremotifier.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mdremotifier
-Version: 0.3.1
+Version: 0.3.2
 Summary: Remotify local links in README.md.
 Author-email: AYF <realazthat@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Azriel Fasten.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
@@ -91,14 +91,15 @@
 Requires-Dist: jaraco-functools==4.0.1; extra == "dev"
 Requires-Dist: jeepney==0.8.0; extra == "dev"
 Requires-Dist: jinja2==3.1.3; extra == "dev"
 Requires-Dist: keyring==25.2.0; extra == "dev"
 Requires-Dist: markdown-it-py==3.0.0; extra == "dev"
 Requires-Dist: markupsafe==2.1.5; extra == "dev"
 Requires-Dist: mdurl==0.1.2; extra == "dev"
+Requires-Dist: mdreftidy==0.3.0; extra == "dev"
 Requires-Dist: mistletoe==1.3.0; extra == "dev"
 Requires-Dist: more-itertools==10.2.0; extra == "dev"
 Requires-Dist: mypy==1.8.0; extra == "dev"
 Requires-Dist: mypy-extensions==1.0.0; extra == "dev"
 Requires-Dist: nh3==0.2.17; extra == "dev"
 Requires-Dist: nodeenv==1.8.0; extra == "dev"
 Requires-Dist: pathspec==0.12.1; extra == "dev"
@@ -201,64 +202,67 @@
 |                   | Status                      | Stable                    | Unstable                  |                    |
 | ----------------- | --------------------------- | ------------------------- | ------------------------- | ------------------ |
 | **[Master][10]**  | [![Build and Test][11]][12] | [![since tagged][13]][14] |                           | ![last commit][15] |
 | **[Develop][16]** | [![Build and Test][17]][12] | [![since tagged][18]][19] | [![since tagged][20]][21] | ![last commit][22] |
 
 </div>
 
-<img alt="Demo" src="https://raw.githubusercontent.com/realazthat/mdremotifier/v0.3.1/.github/demo.gif" width="100%"/>
+<img alt="Demo" src="https://raw.githubusercontent.com/realazthat/mdremotifier/v0.3.2/.github/demo.gif" width="100%"/>
 
 ## ❔ What
 
 What mdremotifier does:
 
-Turn this ([./mdremotifier/examples/EXAMPLE.md](https://github.com/realazthat/mdremotifier/blob/v0.3.1/mdremotifier/examples/EXAMPLE.md)):
+Turn this ([./mdremotifier/examples/EXAMPLE.md](https://github.com/realazthat/mdremotifier/blob/v0.3.2/mdremotifier/examples/EXAMPLE.md)):
 
 <!---->
 ```md
 # Example markdown file
 
 A link to a local file [LICENSE.md](./LICENSE.md).
 
 ```
 <!---->
 
 Into this
-([./mdremotifier/examples/EXAMPLE.remotified.md](https://github.com/realazthat/mdremotifier/blob/v0.3.1/mdremotifier/examples/EXAMPLE.remotified.md)):
+([./mdremotifier/examples/EXAMPLE.remotified.md](https://github.com/realazthat/mdremotifier/blob/v0.3.2/mdremotifier/examples/EXAMPLE.remotified.md)):
 
 <!---->
 ```md
 # Example markdown file
 
 A link to a local file [LICENSE.md](https://raw.githubusercontent.com/realazthat/mdremotifier/master/LICENSE.md).
 
 ```
 <!---->
 
 This is useful for uploading `README.md` files to third-party sites, like the
 npmjs.com registry, or pypi.org registry, because these registries will break
 the local images in your README when displayed on their sites.
 
+See <https://pypi.org/project/mdremotifier/>, notice how all of the images are
+not broken.
+
 ## 🎇 Features
 
 - 📷🔗📡🌐🖼️ Replace local URLs with raw.githubusercontent.com URLs.
 
 ## 🏠 Installation
 
 ```bash
 # Install from pypi (https://pypi.org/project/mdremotifier/)
 pip install mdremotifier
 
 # Install from git (https://github.com/realazthat/mdremotifier)
-pip install git+https://github.com/realazthat/mdremotifier.git@v0.3.1
+pip install git+https://github.com/realazthat/mdremotifier.git@v0.3.2
 ```
 
 ## 🚜 Usage
 
-Example README: ([./mdremotifier/examples/EXAMPLE.md](https://github.com/realazthat/mdremotifier/blob/v0.3.1/mdremotifier/examples/EXAMPLE.md)):
+Example README: ([./mdremotifier/examples/EXAMPLE.md](https://github.com/realazthat/mdremotifier/blob/v0.3.2/mdremotifier/examples/EXAMPLE.md)):
 
 <!---->
 ```md
 # Example markdown file
 
 A link to a local file [LICENSE.md](./LICENSE.md).
 
@@ -276,29 +280,29 @@
 
 ```
 <!---->
 
 ## 💻 Command Line Options
 
 <!---->
-<img alt="Output of `python -m mdremotifier.cli --help`" src="https://raw.githubusercontent.com/realazthat/mdremotifier/v0.3.1/README.help.generated.svg"/>
+<img alt="Output of `python -m mdremotifier.cli --help`" src="https://raw.githubusercontent.com/realazthat/mdremotifier/v0.3.2/README.help.generated.svg"/>
 <!-- -->
 
 ## 💡 Examples
 
 - mdremotifier's own `README`:
-  - Original: [./README.md](https://github.com/realazthat/mdremotifier/blob/v0.3.1/README.md).
-  - Remotified: [./.github/README.remotified.md](https://github.com/realazthat/mdremotifier/blob/v0.3.1/.github/README.remotified.md).
-  - Generation script: [./scripts/generate-readme.sh](https://github.com/realazthat/mdremotifier/blob/v0.3.1/scripts/generate-readme.sh).
+  - Original: [./README.md](https://github.com/realazthat/mdremotifier/blob/v0.3.2/README.md).
+  - Remotified: [./.github/README.remotified.md](https://github.com/realazthat/mdremotifier/blob/v0.3.2/.github/README.remotified.md).
+  - Generation script: [./scripts/generate-readme.sh](https://github.com/realazthat/mdremotifier/blob/v0.3.2/scripts/generate-readme.sh).
 - Example:
-  - Original: [./mdremotifier/examples/EXAMPLE.md](https://github.com/realazthat/mdremotifier/blob/v0.3.1/mdremotifier/examples/EXAMPLE.md).
+  - Original: [./mdremotifier/examples/EXAMPLE.md](https://github.com/realazthat/mdremotifier/blob/v0.3.2/mdremotifier/examples/EXAMPLE.md).
   - Remotified:
-    [./mdremotifier/examples/EXAMPLE.remotified.md](https://github.com/realazthat/mdremotifier/blob/v0.3.1/mdremotifier/examples/EXAMPLE.remotified.md).
+    [./mdremotifier/examples/EXAMPLE.remotified.md](https://github.com/realazthat/mdremotifier/blob/v0.3.2/mdremotifier/examples/EXAMPLE.remotified.md).
   - Generation script:
-    [./mdremotifier/examples/example.sh](https://github.com/realazthat/mdremotifier/blob/v0.3.1/mdremotifier/examples/example.sh).
+    [./mdremotifier/examples/example.sh](https://github.com/realazthat/mdremotifier/blob/v0.3.2/mdremotifier/examples/example.sh).
 
 <!-- TODO: Rebuild this for mdremotifier
 - Projects using mdremotifier:
   - [realazthat/snipinator](https://github.com/realazthat/snipinator), See
     [snipinator/README.md.jinja2](https://github.com/realazthat/snipinator/blob/61cb88593baa099dc375cf5fd40679e4be673fc5/README.md.jinja2).
   - [github.com/realazthat/changeguard](https://github.com/realazthat/changeguard),
     See
@@ -321,25 +325,25 @@
 - Python 3.8+
   - Why: Some dev dependencies require Python 3.8+.
 
 ### Tested Platforms
 
 - WSL2 Ubuntu 20.04, Python `3.8.0`.
 - Ubuntu 20.04, Python `3.8.0, 3.9.0, 3.10.0, 3.11.0, 3.12.0`, tested in GitHub Actions
-  workflow ([build-and-test.yml](https://github.com/realazthat/mdremotifier/blob/v0.3.1/.github/workflows/build-and-test.yml)).
+  workflow ([build-and-test.yml](https://github.com/realazthat/mdremotifier/blob/v0.3.2/.github/workflows/build-and-test.yml)).
 
 ## 🤏 Versioning
 
 We use SemVer for versioning. For the versions available, see the tags on this
 repository.
 
 ## 🔑 License
 
 This project is licensed under the MIT License - see the
-[./LICENSE.md](https://github.com/realazthat/mdremotifier/blob/v0.3.1/LICENSE.md) file for details.
+[./LICENSE.md](https://github.com/realazthat/mdremotifier/blob/v0.3.2/LICENSE.md) file for details.
 
 ## 🙏 Thanks
 
 Main libraries used in mdremotifier are:
 
 - Markdown AST: [mistletoe](https://github.com/miyuchina/mistletoe).
 - Colorful CLI help: [rich-argparse](https://github.com/hamdanal/rich-argparse).
@@ -363,15 +367,15 @@
 
 ## 🫡 Contributions
 
 ### Development environment: Linux-like
 
 - For running `pre.sh` (Linux-like environment).
 
-  - From [./.github/dependencies.yml](https://github.com/realazthat/mdremotifier/blob/v0.3.1/.github/dependencies.yml), which is used for
+  - From [./.github/dependencies.yml](https://github.com/realazthat/mdremotifier/blob/v0.3.2/.github/dependencies.yml), which is used for
     the GH Action to do a fresh install of everything:
 
     ```yaml
     bash: scripts.
     findutils: scripts.
     grep: tests.
     xxd: tests.
@@ -382,47 +386,47 @@
     jq: dependency for [yq](https://github.com/kislyuk/yq), which is used to generate
       the README; the README generator needs to use `tomlq` (which is a part of `yq`)
       to query `pyproject.toml`.
 
     ```
 
   - Requires `pyenv`, or an exact matching version of python as in
-    [.python-version](https://github.com/realazthat/mdremotifier/blob/v0.3.1/.python-version) (which is currently
+    [.python-version](https://github.com/realazthat/mdremotifier/blob/v0.3.2/.python-version) (which is currently
     `3.8.0 `).
   - `jq`, ([installation](https://jqlang.github.io/jq/)) required for
     [yq](https://github.com/kislyuk/yq), which is itself required for our
-    [./README.md](https://github.com/realazthat/mdremotifier/blob/v0.3.1/README.md) generation, which uses `tomlq` (from the
+    [./README.md](https://github.com/realazthat/mdremotifier/blob/v0.3.2/README.md) generation, which uses `tomlq` (from the
     [yq](https://github.com/kislyuk/yq) package) to include version strings from
-    [./pyproject.toml](https://github.com/realazthat/mdremotifier/blob/v0.3.1/pyproject.toml).
+    [./pyproject.toml](https://github.com/realazthat/mdremotifier/blob/v0.3.2/pyproject.toml).
   - act (to run the GH Action locally):
     - Requires nodejs.
     - Requires Go.
     - docker.
   - Generate animation:
     - docker
 
 ### Commit Process
 
 1. (Optionally) Fork the `develop` branch.
 2. Stage your files: `git add path/to/file.py`.
 3. `bash ./scripts/pre.sh`, this will format, lint, and test the code.
 4. `git status` check if anything changed (generated
-   [./README.md](https://github.com/realazthat/mdremotifier/blob/v0.3.1/README.md) for example), if so, `git add` the
+   [./README.md](https://github.com/realazthat/mdremotifier/blob/v0.3.2/README.md) for example), if so, `git add` the
    changes, and go back to the previous step.
 5. `git commit -m "..."`.
 6. Make a PR to `develop` (or push to develop if you have the rights).
 
 ## 🔄🚀 Release Process
 
 These instructions are for maintainers of the project.
 
 1. In the `develop` branch, run `bash ./scripts/pre.sh` to ensure
    everything is in order.
 2. In the `develop` branch, bump the version in
-   [./pyproject.toml](https://github.com/realazthat/mdremotifier/blob/v0.3.1/pyproject.toml), following semantic versioning
+   [./pyproject.toml](https://github.com/realazthat/mdremotifier/blob/v0.3.2/pyproject.toml), following semantic versioning
    principles. Also modify the `last_unstable_release` and `last_stable_release`
    in the `[tool.mdremotifier-project-metadata]` table as appropriate. Run
    `bash ./scripts/pre.sh` to ensure everything is in order.
 3. In the `develop` branch, commit these changes with a message like
    `"Prepare release X.Y.Z"`. (See the contributions section
    [above](#commit-process)).
 4. Merge the `develop` branch into the `master` branch:
@@ -434,35 +438,35 @@
 7. Push to GitHub: Push the commit and tags to GitHub with
    `git push && git push --tags`.
 8. The `--no-ff` option adds a commit to the master branch for the merge, so
    refork the develop branch from the master branch:
    `git checkout develop && git merge master`.
 9. Push the develop branch to GitHub: `git push origin develop`.
 
-[1]: https://raw.githubusercontent.com/realazthat/mdremotifier/v0.3.1/.github/logo-exported.svg
+[1]: https://raw.githubusercontent.com/realazthat/mdremotifier/v0.3.2/.github/logo-exported.svg
 [2]: https://img.shields.io/badge/Audience-Developers-0A1E1E?style=plastic&logo=data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIyNCIgaGVpZ2h0PSIyNCIgdmlld0JveD0iMCAwIDI0IDI0IiBmaWxsPSJub25lIiBzdHJva2U9ImN1cnJlbnRDb2xvciIgc3Ryb2tlLXdpZHRoPSIyIiBzdHJva2UtbGluZWNhcD0icm91bmQiIHN0cm9rZS1saW5lam9pbj0icm91bmQiIGNsYXNzPSJsdWNpZGUgbHVjaWRlLXVzZXJzIj48cGF0aCBkPSJNMTYgMjF2LTJhNCA0IDAgMCAwLTQtNEg2YTQgNCAwIDAgMC00IDR2MiIvPjxjaXJjbGUgY3g9IjkiIGN5PSI3IiByPSI0Ii8+PHBhdGggZD0iTTIyIDIxdi0yYTQgNCAwIDAgMC0zLTMuODciLz48cGF0aCBkPSJNMTYgMy4xM2E0IDQgMCAwIDEgMCA3Ljc1Ii8+PC9zdmc+
 [3]: https://img.shields.io/badge/Platform-Linux-0A1E1E?style=plastic&logo=data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIyNCIgaGVpZ2h0PSIyNCIgdmlld0JveD0iMCAwIDI0IDI0IiBmaWxsPSJub25lIiBzdHJva2U9ImN1cnJlbnRDb2xvciIgc3Ryb2tlLXdpZHRoPSIyIiBzdHJva2UtbGluZWNhcD0icm91bmQiIHN0cm9rZS1saW5lam9pbj0icm91bmQiIGNsYXNzPSJsdWNpZGUgbHVjaWRlLWxhcHRvcC1taW5pbWFsIj48cmVjdCB3aWR0aD0iMTgiIGhlaWdodD0iMTIiIHg9IjMiIHk9IjQiIHJ4PSIyIiByeT0iMiIvPjxsaW5lIHgxPSIyIiB4Mj0iMjIiIHkxPSIyMCIgeTI9IjIwIi8+PC9zdmc+
 [4]: https://img.shields.io/github/languages/top/realazthat/mdremotifier.svg?&cacheSeconds=28800&style=plastic&color=0A1E1E
 [5]: https://img.shields.io/github/license/realazthat/mdremotifier?style=plastic&color=0A1E1E
-[6]: https://github.com/realazthat/mdremotifier/blob/v0.3.1/LICENSE.md
+[6]: https://github.com/realazthat/mdremotifier/blob/v0.3.2/LICENSE.md
 [7]: https://img.shields.io/pypi/v/mdremotifier?style=plastic&color=0A1E1E
 [8]: https://pypi.org/project/mdremotifier/
 [9]: https://img.shields.io/pypi/pyversions/mdremotifier?style=plastic&color=0A1E1E
 [10]: https://github.com/realazthat/mdremotifier/tree/master
 [11]: https://img.shields.io/github/actions/workflow/status/realazthat/mdremotifier/build-and-test.yml?branch=master&style=plastic
 [12]: https://github.com/realazthat/mdremotifier/actions/workflows/build-and-test.yml
-[13]: https://img.shields.io/github/commits-since/realazthat/mdremotifier/v0.3.1/master?style=plastic
-[14]: https://github.com/realazthat/mdremotifier/compare/v0.3.1...master
+[13]: https://img.shields.io/github/commits-since/realazthat/mdremotifier/v0.3.2/master?style=plastic
+[14]: https://github.com/realazthat/mdremotifier/compare/v0.3.2...master
 [15]: https://img.shields.io/github/last-commit/realazthat/mdremotifier/master?style=plastic
 [16]: https://github.com/realazthat/mdremotifier/tree/develop
 [17]: https://img.shields.io/github/actions/workflow/status/realazthat/mdremotifier/build-and-test.yml?branch=develop&style=plastic
-[18]: https://img.shields.io/github/commits-since/realazthat/mdremotifier/v0.3.1/develop?style=plastic
-[19]: https://github.com/realazthat/mdremotifier/compare/v0.3.1...develop
-[20]: https://img.shields.io/github/commits-since/realazthat/mdremotifier/v0.3.1/develop?style=plastic
-[21]: https://github.com/realazthat/mdremotifier/compare/v0.3.1...develop
+[18]: https://img.shields.io/github/commits-since/realazthat/mdremotifier/v0.3.2/develop?style=plastic
+[19]: https://github.com/realazthat/mdremotifier/compare/v0.3.2...develop
+[20]: https://img.shields.io/github/commits-since/realazthat/mdremotifier/v0.3.2/develop?style=plastic
+[21]: https://github.com/realazthat/mdremotifier/compare/v0.3.2...develop
 [22]: https://img.shields.io/github/last-commit/realazthat/mdremotifier/develop?style=plastic
 [23]: https://github.com/bdashore3/remark-github-images "Documentation is non-existent, but code looks very similar to mdremotifier"
 [24]: https://github.com/laobie/WriteMarkdownLazily "Uploads to cloud."
 [25]: https://github.com/crh19970307/mdul "Uploads to sm.ms"
 [26]: https://github.com/SkyLee424/Go-MarkDown-Image-Transfer-Helper "Upload to Qiniu Cloud"
 [27]: https://github.com/jen6/imgo "Upload to Google Drive"
 [28]: https://github.com/chocoluffy/lazy-markdown "Uploads to LeanCloud, readme is a bit unclear"
```

### Comparing `mdremotifier-0.3.1/mdremotifier.egg-info/requires.txt` & `mdremotifier-0.3.2/mdremotifier.egg-info/requires.txt`

 * *Files 5% similar despite different names*

```diff
@@ -39,14 +39,15 @@
 jaraco-functools==4.0.1
 jeepney==0.8.0
 jinja2==3.1.3
 keyring==25.2.0
 markdown-it-py==3.0.0
 markupsafe==2.1.5
 mdurl==0.1.2
+mdreftidy==0.3.0
 mistletoe==1.3.0
 more-itertools==10.2.0
 mypy==1.8.0
 mypy-extensions==1.0.0
 nh3==0.2.17
 nodeenv==1.8.0
 pathspec==0.12.1
```

### Comparing `mdremotifier-0.3.1/pyproject.toml` & `mdremotifier-0.3.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=64", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mdremotifier"
-version = "0.3.1"
+version = "0.3.2"
 description = "Remotify local links in README.md."
 authors = [{name = "AYF", email = "realazthat@gmail.com"}]
 license = {file = "LICENSE.md"}
 readme = ".github/README.remotified.md"
 requires-python = ">=3.8"
 classifiers = [
   "Operating System :: OS Independent",
@@ -93,14 +93,15 @@
   "jaraco-functools==4.0.1",
   "jeepney==0.8.0",
   "jinja2==3.1.3",
   "keyring==25.2.0",
   "markdown-it-py==3.0.0",
   "markupsafe==2.1.5",
   "mdurl==0.1.2",
+  "mdreftidy==0.3.0",
   "mistletoe==1.3.0",
   "more-itertools==10.2.0",
   "mypy==1.8.0",
   "mypy-extensions==1.0.0",
   "nh3==0.2.17",
   "nodeenv==1.8.0",
   "pathspec==0.12.1",
@@ -145,14 +146,14 @@
 
 [project.urls]
 Homepage = "https://github.com/realazthat/mdremotifier"
 Documentation = "https://github.com/realazthat/mdremotifier"
 Repository = "https://github.com/realazthat/mdremotifier"
 
 [tool.mdremotifier-project-metadata]
-last_unstable_release = "0.3.1"
-last_stable_release = "0.3.1"
+last_unstable_release = "0.3.2"
+last_stable_release = "0.3.2"
 
 [tool.setuptools]
 packages = ["mdremotifier"]
 
 [tool.tomlsort]
```

